<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="description" content="Abang Foundation: A Home for Every Heart">
    <title>Meeting the Meek</title>
    <style>
        #dynamicText {
            color: blue;
            font-size: 18px;
        }
        .highlight {
            background-color: yellow;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Abang Foundation</h1>
    <h3>Welcoming the Needy</h3>
    <h6>Bring all your charitable gifts</h6>
    <img src="charity logo.png" alt="Abang Foundation">
    <p id="dynamicText">Welcome to Abang Foundation: A Home for Every Heart</p>

    <button id="changeTextBtn">Change Text</button>
    <button id="toggleStyleBtn">Toggle Highlight</button>
    <button id="addRemoveElementBtn">Add/Remove Element</button>

    <div id="container"></div>

    <script>
        // Change text content dynamically
        document.getElementById('changeTextBtn').addEventListener('click', function() {
            const dynamicText = document.getElementById('dynamicText');
            dynamicText.textContent = "Thank you for supporting Abang Foundation!";
        });

        // Modify CSS styles dynamically
        document.getElementById('toggleStyleBtn').addEventListener('click', function() {
            const dynamicText = document.getElementById('dynamicText');
            dynamicText.classList.toggle('highlight');
        });

        // Add or remove an element dynamically
        document.getElementById('addRemoveElementBtn').addEventListener('click', function() {
            const container = document.getElementById('container');
            const existingElement = document.getElementById('newElement');

            if (existingElement) {
                container.removeChild(existingElement);
            } else {
                const newElement = document.createElement('p');
                newElement.id = 'newElement';
                newElement.textContent = "This is a dynamically added element.";
                container.appendChild(newElement);
            }
        });
    </script>
</body>
<footer>Welcome to Abang Foundation: A Home for Every Heart</footer>
</html>
