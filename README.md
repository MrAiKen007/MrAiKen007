<svg xmlns="http://www.w3.org/2000/svg" width="500" height="320" viewBox="0 0 500 320" fill="none">
  <style>
    .bg { fill: #282A36; }
    .text { fill: white; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; font-size: 18px; }
    .title { font-size: 24px; font-weight: bold; }
    .subtext { font-size: 14px; fill: #BFBFBF; }
    .time { font-size: 20px; fill: #50FA7B; }
    .language { font-size: 18px; fill: #F1FA8C; }
    .circle { stroke-width: 2px; stroke: white; }
    .progress { fill: #6272A4; }
    .progress-bar { fill: #FF79C6; }
  </style>

  <!-- Background -->
  <rect width="500" height="320" class="bg" rx="15"/>

  <!-- Title and Subtitle -->
  <text x="20" y="40" class="text title">👨‍💻 Full Stack Developer</text>
  <text x="20" y="70" class="subtext">Building with C#, Python, JavaScript</text>

  <!-- Current Time -->
  <text x="20" y="110" class="time" id="current-time">🕒 Time: --:--</text>

  <!-- Current Activity -->
  <text x="20" y="150" class="text">📝 Current Activity: Enhancing AI-based App</text>

  <!-- Most Used Languages -->
  <text x="20" y="190" class="text">🔧 Most Used Languages:</text>

  <!-- Language Icons -->
  <g transform="translate(30, 210)">
    <circle cx="20" cy="20" r="20" fill="#5D3FD3" class="circle"/>
    <text x="50" y="25" class="language">C#</text>
  </g>
  <g transform="translate(30, 250)">
    <circle cx="20" cy="20" r="20" fill="#F7DF1E" class="circle"/>
    <text x="50" y="25" class="language">JavaScript</text>
  </g>
  <g transform="translate(30, 290)">
    <circle cx="20" cy="20" r="20" fill="#3776AB" class="circle"/>
    <text x="50" y="25" class="language">Python</text>
  </g>

  <!-- Project Progress Bar -->
  <text x="250" y="190" class="text">🚀 Project Progress:</text>
  <rect x="250" y="210" width="200" height="20" class="progress" rx="10"/>
  <rect x="250" y="210" width="120" height="20" class="progress-bar" rx="10"/>
  <text x="250" y="245" class="text">60% - AI Note Organizer</text>

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
