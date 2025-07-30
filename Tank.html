<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TANKASS - Trash Sorting Game</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #e0f7fa;
            text-align: center;
            margin: 0;
            padding: 20px;
            overflow: hidden;
        }
        
        #game-container {
            max-width: 800px;
            margin: 0 auto;
            background-color: #ffffff;
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        #start-screen {
            margin: 30px 0;
            position: relative;
            z-index: 10;
        }
        
        #game-screen {
            display: none;
            position: relative;
            z-index: 5;
        }
        
        #end-screen {
            display: none;
            margin: 30px 0;
            position: relative;
            z-index: 10;
        }
        
        h1 {
            color: #00796b;
            margin-bottom: 10px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }
        
        h2 {
            color: #00897b;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }
        
        input, button {
            padding: 10px 15px;
            margin: 10px;
            border-radius: 5px;
            border: 1px solid #b2dfdb;
            font-size: 16px;
            position: relative;
            z-index: 20;
        }
        
        button {
            background-color: #00796b;
            color: white;
            border: none;
            cursor: pointer;
            transition: all 0.3s;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }
        
        button:hover {
            background-color: #00695c;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        }
        
        #hud {
            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
            padding: 10px;
            background-color: rgba(178, 223, 219, 0.8);
            border-radius: 10px;
            position: relative;
            z-index: 10;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        #play-area {
            position: relative;
            height: 400px;
            border-radius: 10px;
            overflow: hidden;
        }
        
        #background {
            position: absolute;
            width: 200%;
            height: 100%;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 400"><rect width="800" height="400" fill="%23b3e5fc"/><rect y="300" width="800" height="100" fill="%2381c784"/><path d="M0,300 Q200,250 400,300 T800,300" fill="%2366bb6a" opacity="0.8"/><circle cx="100" cy="100" r="40" fill="%23ffd54f"/><circle cx="300" cy="120" r="30" fill="%23ffd54f"/><circle cx="500" cy="80" r="50" fill="%23ffd54f"/><rect x="50" y="280" width="20" height="80" fill="%235d4037"/><path d="M60,280 Q60,200 80,200 Q100,200 100,280" fill="%234caf50"/><rect x="250" y="260" width="20" height="100" fill="%235d4037"/><path d="M260,260 Q260,180 280,180 Q300,180 300,260" fill="%234caf50"/><rect x="450" y="240" width="20" height="120" fill="%235d4037"/><path d="M460,240 Q460,140 480,140 Q500,140 500,240" fill="%234caf50"/></svg>');
            background-repeat: repeat-x;
            animation: scrollBackground 60s linear infinite;
            z-index: 1;
        }
        
        @keyframes scrollBackground {
            0% { transform: translateX(0); }
            100% { transform: translateX(-50%); }
        }
        
        .environment-item {
            position: absolute;
            z-index: 2;
            pointer-events: none;
        }
        
        .flower {
            width: 30px;
            height: 30px;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 30 30"><circle cx="15" cy="15" r="5" fill="%23fdd835"/><circle cx="8" cy="8" r="4" fill="%23ffeb3b"/><circle cx="22" cy="8" r="4" fill="%23ffeb3b"/><circle cx="8" cy="22" r="4" fill="%23ffeb3b"/><circle cx="22" cy="22" r="4" fill="%23ffeb3b"/><rect x="14" y="15" width="2" height="15" fill="%238bc34a"/></svg>');
            background-size: contain;
        }
        
        .tree {
            width: 60px;
            height: 80px;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 60 80"><rect x="25" y="40" width="10" height="40" fill="%235d4037"/><circle cx="30" cy="20" r="20" fill="%232e7d32"/><circle cx="15" cy="30" r="15" fill="%232e7d32"/><circle cx="45" cy="30" r="15" fill="%232e7d32"/><circle cx="30" cy="40" r="15" fill="%232e7d32"/></svg>');
            background-size: contain;
        }
        
        .trash-item {
            position: absolute;
            width: 60px;
            height: 60px;
            background-size: contain;
            background-repeat: no-repeat;
            background-position: center;
            cursor: pointer;
            transition: all 0.3s;
            z-index: 3;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 30px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
        }
        
        .trash-item:hover {
            transform: scale(1.2) rotate(10deg);
        }
        
        .correct-trash {
            border: 3px solid #4caf50;
            border-radius: 15px;
            background-color: rgba(76, 175, 80, 0.2);
        }
        
        .wrong-trash {
            border: 3px solid #f44336;
            border-radius: 15px;
            background-color: rgba(244, 67, 54, 0.2);
        }
        
        .collected {
            animation: collectAnimation 0.5s forwards;
        }
        
        @keyframes collectAnimation {
            0% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.5); opacity: 0.5; }
            100% { transform: scale(0); opacity: 0; }
        }
        
        #tankass {
            width: 150px;
            height: 150px;
            margin: 20px auto;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="50" cy="50" r="45" fill="%2300796b"/><circle cx="35" cy="40" r="5" fill="white"/><circle cx="65" cy="40" r="5" fill="white"/><path d="M30,65 Q50,75 70,65" stroke="white" stroke-width="3" fill="none"/><path d="M20,20 Q50,0 80,20" stroke="%23ffeb3b" stroke-width="4" fill="none"/></svg>');
            background-size: contain;
            background-repeat: no-repeat;
            transition: all 0.3s;
        }
        
        #tankass:hover {
            transform: scale(1.1) rotate(5deg);
        }
        
        #message {
            font-size: 24px;
            margin: 20px 0;
            color: #00796b;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
            padding: 10px;
            background-color: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
        }
        
        .clean-spot {
            position: absolute;
            width: 100px;
            height: 100px;
            background-color: rgba(129, 199, 132, 0.3);
            border-radius: 50%;
            z-index: 2;
            pointer-events: none;
        }
    </style>
</head>
<body>
    <div id="game-container">
        <h1>TANKASS</h1>
        <h2>Trash Sorting Game</h2>
        
        <!-- Start Screen -->
        <div id="start-screen">
            <p>Help clean up the town by sorting trash correctly before time runs out!</p>
            <input type="text" id="player-name" placeholder="Enter your name" required>
            <button id="start-btn">Start Game</button>
        </div>
        
        <!-- Game Screen -->
        <div id="game-screen">
            <div id="hud">
                <div>Player: <span id="player-display"></span></div>
                <div>Score: <span id="score">0</span></div>
                <div>Lives: <span id="lives">3</span></div>
                <div>Time: <span id="timer">30</span>s</div>
                <div>Trash Left: <span id="trash-left">15</span></div>
            </div>
            
            <div id="play-area">
                <div id="background"></div>
                <!-- Environment items and trash will be added here by JavaScript -->
            </div>
        </div>
        
        <!-- End Screen -->
        <div id="end-screen">
            <div id="tankass"></div>
            <div id="message"></div>
            <div id="final-score"></div>
            <button id="restart-btn">Play Again</button>
        </div>
    </div>

    <script>
        // Game variables
        let playerName = "";
        let score = 0;
        let lives = 3;
        let timeLeft = 30;
        let trashLeft = 15;
        let gameInterval;
        let timerInterval;
        let trashItems = [];
        let environmentItems = [];
        
        const correctTrashItems = [
            "🍌", "🍎", "🥫", "📰", "🧃", "🥤", "📦", "🍊", "🍐", "🥡",
            "🍏", "🍇", "🍓", "🥥", "🥝", "🥭", "🍍", "🥦", "🥬", "🥒"
        ];
        
        const wrongTrashItems = [
            "👟", "📱", "⌨️", "🖱️", "🎮", "💻", "📷", "🔌", "💡", "🔋",
            "🧦", "👓", "🎧", "🕶️", "🧢", "👔", "👗", "👠", "👜", "👛"
        ];
        
        // DOM elements
        const startScreen = document.getElementById("start-screen");
        const gameScreen = document.getElementById("game-screen");
        const endScreen = document.getElementById("end-screen");
        const playerNameInput = document.getElementById("player-name");
        const startBtn = document.getElementById("start-btn");
        const playerDisplay = document.getElementById("player-display");
        const scoreDisplay = document.getElementById("score");
        const livesDisplay = document.getElementById("lives");
        const timerDisplay = document.getElementById("timer");
        const trashLeftDisplay = document.getElementById("trash-left");
        const playArea = document.getElementById("play-area");
        const background = document.getElementById("background");
        const messageDisplay = document.getElementById("message");
        const finalScoreDisplay = document.getElementById("final-score");
        const restartBtn = document.getElementById("restart-btn");
        
        // Event listeners
        startBtn.addEventListener("click", startGame);
        restartBtn.addEventListener("click", restartGame);
        
        // Game functions
        function startGame() {
            if (!playerNameInput.value.trim()) {
                alert("Please enter your name!");
                return;
            }
            
            playerName = playerNameInput.value.trim();
            playerDisplay.textContent = playerName;
            
            // Reset game state
            score = 0;
            lives = 3;
            timeLeft = 30;
            trashLeft = 15;
            
            // Clear any existing items
            trashItems.forEach(item => {
                if (item.element.parentNode === playArea) {
                    playArea.removeChild(item.element);
                }
            });
            trashItems = [];
            
            environmentItems.forEach(item => {
                if (item.parentNode === playArea) {
                    playArea.removeChild(item);
                }
            });
            environmentItems = [];
            
            // Update displays
            scoreDisplay.textContent = score;
            livesDisplay.textContent = lives;
            timerDisplay.textContent = timeLeft;
            trashLeftDisplay.textContent = trashLeft;
            
            // Switch screens
            startScreen.style.display = "none";
            gameScreen.style.display = "block";
            endScreen.style.display = "none";
            
            // Create environment items (flowers and trees)
            createEnvironment();
            
            // Start trash generation
            gameInterval = setInterval(createTrashItem, 1500);
            
            // Start timer
            timerInterval = setInterval(updateTimer, 1000);
            
            // Start animation loop
            requestAnimationFrame(updateGame);
        }
        
        function createEnvironment() {
            // Create flowers
            for (let i = 0; i < 10; i++) {
                const flower = document.createElement("div");
                flower.className = "environment-item flower";
                flower.style.left = `${Math.random() * (playArea.offsetWidth - 30)}px`;
                flower.style.top = `${300 + Math.random() * 70}px`;
                playArea.appendChild(flower);
                environmentItems.push(flower);
            }
            
            // Create trees
            for (let i = 0; i < 5; i++) {
                const tree = document.createElement("div");
                tree.className = "environment-item tree";
                tree.style.left = `${Math.random() * (playArea.offsetWidth - 60)}px`;
                tree.style.top = `${250 + Math.random() * 50}px`;
                playArea.appendChild(tree);
                environmentItems.push(tree);
            }
        }
        
        function createTrashItem() {
            if (trashLeft <= 0) return;
            
            const isCorrect = Math.random() > 0.3; // 70% chance of correct trash
            let trashEmoji;
            
            if (isCorrect) {
                const randomIndex = Math.floor(Math.random() * correctTrashItems.length);
                trashEmoji = correctTrashItems[randomIndex];
            } else {
                const randomIndex = Math.floor(Math.random() * wrongTrashItems.length);
                trashEmoji = wrongTrashItems[randomIndex];
            }
            
            const element = document.createElement("div");
            element.className = `trash-item ${isCorrect ? "correct-trash" : "wrong-trash"}`;
            element.textContent = trashEmoji;
            element.style.left = `${Math.random() * (playArea.offsetWidth - 60)}px`;
            element.style.top = `${Math.random() * (playArea.offsetHeight - 60)}px`;
            
            element.addEventListener("click", () => handleTrashClick(element, isCorrect));
            
            playArea.appendChild(element);
            
            // Create trash item object with movement properties
            const trashItem = {
                element: element,
                isCorrect: isCorrect,
                x: Math.random() * (playArea.offsetWidth - 60),
                y: Math.random() * (playArea.offsetHeight - 60),
                vx: (Math.random() - 0.5) * 2,
                vy: (Math.random() - 0.5) * 2,
                rotation: Math.random() * 360,
                rotationSpeed: (Math.random() - 0.5) * 10
            };
            
            trashItems.push(trashItem);
        }
        
        function handleTrashClick(element, isCorrect) {
            if (element.classList.contains("collected")) return;
            
            element.classList.add("collected");
            
            if (isCorrect) {
                // Correct trash clicked
                score++;
                scoreDisplay.textContent = score;
                trashLeft--;
                trashLeftDisplay.textContent = trashLeft;
                
                // Create a clean spot effect
                const cleanSpot = document.createElement("div");
                cleanSpot.className = "clean-spot";
                cleanSpot.style.left = `${parseInt(element.style.left) - 20}px`;
                cleanSpot.style.top = `${parseInt(element.style.top) - 20}px`;
                playArea.appendChild(cleanSpot);
                
                // Remove clean spot after animation
                setTimeout(() => {
                    if (cleanSpot.parentNode === playArea) {
                        playArea.removeChild(cleanSpot);
                    }
                }, 1000);
                
                // Check win condition
                if (trashLeft <= 0) {
                    endGame(true);
                    return;
                }
            } else {
                // Wrong trash clicked
                lives--;
                livesDisplay.textContent = lives;
                
                // Check lose condition
                if (lives <= 0) {
                    endGame(false);
                    return;
                }
            }
            
            // Remove the item after animation
            setTimeout(() => {
                if (element.parentNode === playArea) {
                    playArea.removeChild(element);
                    
                    // Remove from trashItems array
                    const index = trashItems.findIndex(item => item.element === element);
                    if (index !== -1) {
                        trashItems.splice(index, 1);
                    }
                }
            }, 500);
        }
        
        function updateTimer() {
            timeLeft--;
            timerDisplay.textContent = timeLeft;
            
            if (timeLeft <= 0) {
                endGame(false);
            }
        }
        
        function updateGame() {
            // Update trash item positions
            trashItems.forEach(item => {
                // Update position
                item.x += item.vx;
                item.y += item.vy;
                
                // Bounce off walls
                if (item.x <= 0 || item.x >= playArea.offsetWidth - 60) {
                    item.vx *= -1;
                }
                if (item.y <= 0 || item.y >= playArea.offsetHeight - 60) {
                    item.vy *= -1;
                }
                
                // Update rotation
                item.rotation += item.rotationSpeed;
                
                // Apply transformations
                item.element.style.left = `${item.x}px`;
                item.element.style.top = `${item.y}px`;
                item.element.style.transform = `rotate(${item.rotation}deg) scale(${item.element.classList.contains("collected") ? 0 : 1})`;
            });
            
            // Continue animation loop if game is still running
            if (gameScreen.style.display === "block") {
                requestAnimationFrame(updateGame);
            }
        }
        
        function endGame(isWin) {
            clearInterval(gameInterval);
            clearInterval(timerInterval);
            
            gameScreen.style.display = "none";
            endScreen.style.display = "block";
            
            if (isWin) {
                messageDisplay.textContent = `You Win, ${playerName}! Well done! You cleaned it all up!`;
                messageDisplay.style.color = "#4caf50";
            } else {
                messageDisplay.textContent = `Game Over, ${playerName}! TANKASS says… try again and sort better next time!`;
                messageDisplay.style.color = "#f44336";
            }
            
            finalScoreDisplay.textContent = `Your final score: ${score}`;
        }
        
        function restartGame() {
            endScreen.style.display = "none";
            startScreen.style.display = "block";
        }
    </script>
</body>
</html>
