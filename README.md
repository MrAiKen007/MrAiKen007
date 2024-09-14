<svg xmlns="http://www.w3.org/2000/svg" width="500" height="300" viewBox="0 0 500 300" fill="none">
  <style>
    .bg { fill: #1E1E2F; }
    .text { fill: white; font-family: 'Arial', sans-serif; font-size: 18px; }
    .time { font-size: 24px; }
    .icon { fill: white; font-size: 24px; }
    .circle { stroke: #FFD700; stroke-width: 4px; }
  </style>
  
  <!-- Background -->
  <rect width="500" height="300" class="bg" rx="15"/>
  
  <!-- Title -->
  <text x="20" y="40" class="text" font-size="28px">👨‍💻 Full Stack Developer</text>
  
  <!-- Current Time -->
  <text x="20" y="80" class="text time" id="current-time">🕒 Time: --:--</text>

  <!-- Activity Section -->
  <text x="20" y="120" class="text">📝 Current Activity: Building AI-enhanced App</text>

  <!-- Languages Used -->
  <text x="20" y="160" class="text">🔧 Most Used Languages:</text>
  <g transform="translate(20, 180)">
    <circle cx="20" cy="20" r="20" fill="#5D3FD3"/>
    <text x="45" y="25" class="text">C#</text>
  </g>
  <g transform="translate(20, 220)">
    <circle cx="20" cy="20" r="20" fill="#FFD700"/>
    <text x="45" y="25" class="text">JavaScript</text>
  </g>
  <g transform="translate(20, 260)">
    <circle cx="20" cy="20" r="20" fill="#3776AB"/>
    <text x="45" y="25" class="text">Python</text>
  </g>

  <!-- Progress on Projects -->
  <text x="250" y="160" class="text">🚀 Project Progress:</text>
  <rect x="250" y="180" width="200" height="20" rx="10" fill="#FFD700" />
  <rect x="250" y="180" width="100" height="20" rx="10" fill="#1E90FF" />
  <text x="250" y="215" class="text">50% - AI Note Organizer</text>

  <!-- Script to Show Time -->
  <script type="text/javascript">
    function updateTime() {
      var now = new Date();
      var hours = now.getHours();
      var minutes = now.getMinutes();
      if (minutes < 10) { minutes = '0' + minutes; }
      document.getElementById('current-time').textContent = '🕒 Time: ' + hours + ':' + minutes;
    }
    setInterval(updateTime, 1000);
    updateTime();
  </script>
</svg>
