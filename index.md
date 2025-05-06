<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="description" content="CrawlMacOS: A GPT-4-Based Framework for Autonomous macOS UI Exploration">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>CrawlMacOS: GPT-4-Based macOS UI Agent</title>

  <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro" rel="stylesheet">
  <link rel="stylesheet" href="./static/css/bulma.min.css">
  <link rel="stylesheet" href="./static/css/fontawesome.all.min.css">
  <link rel="stylesheet" href="./static/css/index.css">
  <link rel="icon" href="./static/images/favicon.svg">
</head>
<body>

<!-- Hero Section -->
<section class="hero teaser">
  <div class="container is-max-desktop">
    <div class="hero-body has-text-centered">
      <img src="images/banner.png" alt="Banner Image" style="max-width: 100%;">
      <h2 class="subtitle has-text-centered mt-4">
        <strong>CrawlMacOS</strong> is a fully automated framework for exploring macOS applications via the accessibility API. It generates a large-scale dataset of full-desktop screenshots, interaction graphs, and task specifications, enabling research in complex, multi-window desktop agents.
      </h2>
    </div>
  </div>
</section>

<!-- Abstract Section -->
<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          <p>
            We introduce <strong>CrawlMacOS</strong>, a GPT-4-guided autonomous framework for systematically exploring and interacting with macOS applications via the accessibility API. Our system captures structured UI representations through full-desktop screenshots and rich interaction graphs, generating a benchmark dataset for training and evaluating general-purpose desktop agents.
          </p>
          <p>
            CrawlMacOS autonomously launches apps, interprets accessible UI trees, interacts with interface elements based on natural language guidance, and logs resulting state transitions. This results in a dataset that includes screenshot-state pairs, UI metadata, and task execution traces—enabling novel research in macOS agent reasoning, planning, and perception.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Crawling Pipeline / Methods Section -->
<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Methods: Autonomous Crawling Pipeline</h2>
        <div class="content has-text-justified">
          <p>
            The core component of our framework is a <strong>GPT-4 agent</strong> that autonomously explores macOS apps. The agent parses app UI hierarchies, generates and ranks possible actions using LLM reasoning, performs actions via the macOS accessibility API, and records the resulting UI transitions.
          </p>
          <ul>
            <li><strong>Action Proposal:</strong> LLM proposes plausible UI actions based on current UI state</li>
            <li><strong>Execution & Observation:</strong> Executes action and captures new screenshots/UI tree</li>
            <li><strong>Graph Construction:</strong> Builds structured interaction graphs from state transitions</li>
          </ul>
          <img src="images/Crawler.png" alt="Crawling Pipeline Diagram" style="max-width: 100%; margin-top: 1em;">
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Dataset Section -->
<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Dataset Overview</h2>
        <div class="content has-text-justified">
          <p>
            The <strong>CrawlMacOS</strong> dataset includes structured samples from real macOS apps:
          </p>
          <ul>
            <li><strong>Applications:</strong> 50+ native macOS applications</li>
            <li><strong>Tasks:</strong> 10K+ full interaction steps across contexts</li>
            <li><strong>Data Format:</strong> (Screenshot, Accessibility Tree, Action Metadata, UI Graph)</li>
          </ul>
          <p>
            This dataset enables benchmarking for desktop agents on macOS tasks involving multi-window coordination, memory, and real-world interfaces.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Media Section -->
<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered has-text-centered">
      <div class="column is-one-third">
        <img src="assets/Session.gif" alt="CrawlMacOS Session" style="max-width: 100%;">
      </div>
      <div class="column is-one-third">
        <img src="assets/Reminders.gif" alt="CrawlMacOS Reminders" style="max-width: 100%;">
      </div>
      <div class="column is-one-third">
        <img src="assets/Stocks.gif" alt="CrawlMacOS Stocks" style="max-width: 100%;">
      </div>
    </div>
  </div>
</section>

<!-- Footer Section -->
<footer class="footer">
  <div class="container">
    <div class="content has-text-centered">
      <p>
        © 2025 CrawlMacOS Project. Built for reproducible, open research on macOS agents.
      </p>
      <p>
        <a href="#">[Download Dataset]</a> | <a href="#">[Read the Paper]</a> | <a href="https://github.com/your-repo">[Code]</a>
      </p>
      <p>
            This website is licensed under a <a rel="license"
                                                href="http://creativecommons.org/licenses/by-sa/4.0/">Creative
            Commons Attribution-ShareAlike 4.0 International License</a>.
      </p>
      <p>
      This means you are free to borrow the <a
        href="https://github.com/nerfies/nerfies.github.io">source code</a> of this website,
      we just ask that you link back to this page in the footer.
    </p>
    </div>
  </div>
</footer>

</body>
</html>
