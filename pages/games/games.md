## Asteroids

<style>
    body {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    #game_canvas {
        height: 90vh !important; 
        width: 180vh !important;

        max-width: 95vw;
        object-fit: contain; 
    }
</style>

<body>
    <button id="laser_button" hidden></button>
    <button id="explosion_button" hidden></button>
    <button id="bonus_button" hidden></button>
    <button id="defeat_button" hidden></button>
    <button id="damage_button" hidden></button>
    <button id="bomb_button" hidden></button>
    <canvas id="game_canvas" width="1800" height="900"></canvas>
    <div id="console"></div>
    <script type="text/javascript" src="resources/scripts/audio.js"></script>
    <script type="text/javascript" src="prog/game_js.bc.js"></script>
    <script type="text/javascript">
        window.addEventListener('keydown', function(e) {
            if(e.code === "Space" && e.target === document.body) {
                e.preventDefault();
            }
        });
    </script>
</body>

### Controls

<div style="display: flex; justify-content: center;">
  <table style="text-align: center; border-collapse: collapse; width: 50%; max-width: 400px;">
    <thead>
      <tr>
        <th style="padding: 12px;">Actions</th>
        <th style="padding: 12px;">Keys</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>Up</td><td>Z</td></tr>
      <tr><td>Down</td><td>S</td></tr>
      <tr><td>Left</td><td>Q</td></tr>
      <tr><td>Right</td><td>D</td></tr>
      <tr><td>Fire</td><td>Space</td></tr>
      <tr><td>Pause</td><td>M + Esc</td></tr>
      <tr><td>Resume</td><td>P + Esc</td></tr>
      <tr><td>Quit</td><td>M + &</td></tr>
      <tr><td>Enable God Mode</td><td>M + é</td></tr>
      <tr><td>Disable God Mode</td><td>P + é</td></tr>
      <tr><td>Enable Max Bonus</td><td>M + "</td></tr>
      <tr><td>Disable Max Bonus</td><td>P + "</td></tr>
    </tbody>
  </table>
</div>

### Source Code

<p style="text-align: justify;">
Written in <a href="https://en.wikipedia.org/wiki/OCaml">OCaml</a>. You can find the source code for this game on <a href="https://github.com/hjbar/jeu_asteroids">GitHub</a>.
</p>
