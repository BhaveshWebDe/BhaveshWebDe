<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sphere Volume Calculator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin: 50px;
    }

    h2 {
      color: #333;
    }

    form {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    label {
      margin-bottom: 10px;
    }

    input {
      padding: 8px;
      margin-bottom: 20px;
    }

    button {
      padding: 10px;
      background-color: #3498db;
      color: #fff;
      border: none;
      cursor: pointer;
    }

    #result {
      margin-top: 20px;
      font-weight: bold;
      color: #27ae60;
    }
  </style>
</head>
<body>

<h2>Sphere Volume Calculator</h2>

<form id="sphereForm">
  <label for="radius">Enter the radius of the sphere:</label>
  <input type="number" id="radius" required>
  <button type="button" onclick="calculateVolume()">Calculate Volume</button>
</form>

<p id="result"></p>

<script>
  function calculateVolume() {
    const radiusInput = document.getElementById('radius');
    const resultElement = document.getElementById('result');

    // Get the radius value from the input field
    const radius = parseFloat(radiusInput.value);

    // Check if the input is a valid number
    if (isNaN(radius)) {
      resultElement.textContent = 'Please enter a valid number for the radius.';
      return;
    }

    // Calculate the volume of the sphere
    const pi = Math.PI;
    const volume = (4 / 3) * pi * Math.pow(radius, 3);

    // Display the result
    resultElement.textContent = `The volume of the sphere with radius ${radius} is: ${volume.toFixed(2)}`;
  }
</script>

</body>
</html>
- 👋 Hi, I’m @BhaveshWebDe
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
BhaveshWebDe/BhaveshWebDe is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
