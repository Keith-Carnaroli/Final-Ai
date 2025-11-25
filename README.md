<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tech Knowledge Hub</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f4f4f4;
    }
    header {
      background-color: #333;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    nav {
      display: flex;
      flex-wrap: wrap;
      background-color: #444;
    }
    nav button {
      flex: 1;
      padding: 1rem;
      border: none;
      background-color: #444;
      color: white;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    nav button:hover {
      background-color: #555;
    }
    .content {
      padding: 2rem;
      background-color: white;
      min-height: 300px;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <header>
    <h1>Tech Knowledge Hub</h1>
  </header>

  <nav>
    <button onclick="showSection('brainstorming')">Brainstorming & Computer History</button>
    <button onclick="showSection('dataStorage')">Data Storage</button>
    <button onclick="showSection('database')">Database</button>
    <button onclick="showSection('web')">Web (HTML, CSS, JS)</button>
    <button onclick="showSection('programming')">Programming</button>
    <button onclick="showSection('algorithms')">Algorithms</button>
    <button onclick="showSection('dataManipulation')">Data Manipulation</button>
    <button onclick="showSection('networks')">Networks</button>
    <button onclick="showSection('ai')">AI</button>
  </nav>

  <div class="content">
    <div id="brainstorming">
      <h2>Brainstorming & Computer History</h2>
      <p>Brainstorming helps generate ideas; computer history covers milestones from early machines to modern computers.</p>
    </div>
    <div id="dataStorage" class="hidden">
      <h2>Data Storage</h2>
      <p>Data storage includes HDDs, SSDs, optical media, and cloud storage solutions.</p>
    </div>
    <div id="database" class="hidden">
      <h2>Database</h2>
      <p>Databases organize data for efficient access and management, using models like SQL and NoSQL.</p>
    </div>
    <div id="web" class="hidden">
      <h2>Web (HTML, CSS, JS)</h2>
      <p>The web uses HTML for structure, CSS for styling, and JavaScript for interactivity.</p>
    </div>
    <div id="programming" class="hidden">
      <h2>Programming</h2>
      <p>Programming is the process of writing code to solve problems or create applications.</p>
    </div>
    <div id="algorithms" class="hidden">
      <h2>Algorithms</h2>
      <p>Algorithms are step-by-step procedures for solving problems efficiently.</p>
    </div>
    <div id="dataManipulation" class="hidden">
      <h2>Data Manipulation</h2>
      <p>Data manipulation includes transforming, cleaning, and analyzing data for insights.</p>
    </div>
    <div id="networks" class="hidden">
      <h2>Networks</h2>
      <p>Networks connect computers for communication, using protocols, routers, switches, and more.</p>
    </div>
    <div id="ai" class="hidden">
      <h2>Artificial Intelligence (AI)</h2>
      <p>AI enables machines to perform tasks that typically require human intelligence.</p>
    </div>
  </div>

  <script>
    function showSection(sectionId) {
      const sections = document.querySelectorAll('.content > div');
      sections.forEach(section => {
        section.classList.add('hidden');
      });
      document.getElementById(sectionId).classList.remove('hidden');
    }
  </script>
</body>
</html>
