<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Project Name Generator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      text-align: center;
      padding-top: 100px;
    }
    h1 {
      font-size: 2.5rem;
    }
    #name {
      font-size: 2rem;
      margin: 20px;
      color: #333;
    }
    button {
      padding: 10px 20px;
      font-size: 1.2rem;
      background: #007bff;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }
    button:hover {
      background: #0056b3;
    }
  </style>
</head>
<body>

  <h1>Project Name Generator</h1>
  <div id="name">Click the button to generate a name</div>
  <button onclick="generateName()">Generate</button>

  <script>
    const adjectives = ["Epic", "Silent", "Smart", "Brave", "Quantum", "Electric", "Mystic", "Dynamic", "Rapid", "Infinite"];
    const nouns = ["Falcon", "Nova", "Core", "Storm", "Matrix", "Pulse", "Vortex", "Spark", "Vision", "Beacon"];

    function generateName() {
      const adj = adjectives[Math.floor(Math.random() * adjectives.length)];
      const noun = nouns[Math.floor(Math.random() * nouns.length)];
      document.getElementById("name").innerText = `${adj} ${noun}`;
    }
  </script>

</body>
</html>
