<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TTS TO STT</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="a">
     <a href="tts.html"> <h1>TTS - Text to speech (textni ovozli habarga aylantirish)</h1>  </a>
    </div>
    <div class="b">
        <a href="stt.html"><h1>STT - Speech to text (ovozli habarni textga aylantirish)</h1></a>
    </div>
    <div class="c">
        <a href="need.html"><h1>Eng kerakli 3 ta ovozli habarlar</h1></a>
    </div>
</body>
</html>


<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eng Kerakli Ovozli Habarlar</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #2c3e50;
            color: #fff;
            margin: 0;
            padding: 0;
        }

        h1 {
            text-align: center;
            margin-top: 20px;
            color: #f39c12;
            font-size: 2.5em;
        }

        .container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            padding: 20px;
            justify-items: center;
        }

        .card {
            background-color: #34495e;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: scale(1.05);
        }

        .card button {
            background-color: #f39c12;
            color: white;
            border: none;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.2em;
            transition: background-color 0.3s ease;
        }

        .card button:hover {
            background-color: #e67e22;
        }

        audio {
            display: none;
        }

        .card p {
            font-size: 1.2em;
            color: #ecf0f1;
        }
    </style>
</head>
<body>

    <h1>Eng Kerakli 3 ta Ovozli Habarlar</h1>
    
    <div class="container">
        <div class="card">
            <p>TELEFONGA GAPIRING!</p>
            <button onclick="playAudio('audio/salomalashish.mp3')">BOSING</button>
            <audio id="audio/salomalashish.mp3">
                <source src="Mp3 Editor_241201014226.mp3" type="audio/mp3">
            </audio>
        </div>

        <div class="card">
            <p>BEKAT NOMI NIMA?</p>
            <button onclick="playAudio('audio/qutlash.mp3')">BOSING</button>
            <audio id="audio/qutlash.mp3">
                <source src="Mp3 Editor_241201014529.mp3" type="audio/mp3">
            </audio>
        </div>

        <!-- Qo'shimcha ovozli habarlar -->
        <div class="card">
            <p>KIM OXIRGISI?</p>
            <button onclick="playAudio('audio/shodlik.mp3')">BOSING</button>
            <audio id="audio/shodlik.mp3">
                <source src="Mp3 Editor_241201014318.mp3" type="audio/mp3">
            </audio>
        </div>

        <!-- Ko'proq ovozli habarlarni shu tarzda qo'shishingiz mumkin -->
        
    </div>

    <script>
        function playAudio(audioId) {
            var audio = document.getElementById(audioId);
            audio.play();
        }
    </script>

</body>
</html>




<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ovozli Matn Tizimi (STT)</title>
    <link rel="stylesheet" href="stt.css">
</head>
<body>
    <div class="container">
        <h1>Ovozli Matn Tizimi</h1>
        <div class="stt-box">
            <button id="start-btn">Boshlash</button>
            <button id="stop-btn" disabled>To'xtatish</button>
        </div>
        <div class="output">
            <h2>Natija:</h2>
            <p id="text-output">Ovozli matnni kuting...</p>
        </div>
    </div>
    <script src="stt.js"></script>
</body>
</html>





<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Text to Speech - TTS</title>
    <link rel="stylesheet" href="tts.css">
</head>
<body>
    <div class="container">
        <h1>Text to Speech (TTS)</h1>
        <textarea id="text-input" placeholder="Matnni kiriting..."></textarea>
        
        <div class="controls">
            <select id="voice-select"></select>
            <select id="rate-select">
                <option value="0.5">Ajoyib past tezlik</option>
                <option value="1" selected>O'rtacha tezlik</option>
                <option value="1.5">Tez tezlik</option>
            </select>
            <select id="pitch-select">
                <option value="0.5">Past ton</option>
                <option value="1" selected>O'rtacha ton</option>
                <option value="2">Yuqaridan ton</option>
            </select>
            <button id="speak-btn">Ovoz chiqarish</button>
        </div>

        <p id="status"></p>
    </div>

    <script src="tts.js"></script>
</body>
</html>



body{
    background-color: rgb(41, 12, 12);
    display: flex;
    margin: 10px;
    margin-top: 40px;
  
}
.a{
    text-align: center;
    border: 7px solid white;
    border-radius: 10%;
    background-color: chartreuse;
    width: 20%;
    margin-right: 35px;
    margin-left: 90px;
    text-decoration: none;
}
.b{
    text-align: center;
    border: 7px solid white;
    border-radius: 10%;
    background-color: chartreuse;
    width: 20%;
}
.c{
    text-align: center;
    border: 7px solid white;
    border-radius: 10%;
    background-color: chartreuse;
    width: 20%;
    padding-top: 7px;
    margin-left: 35px;
}





/* Global settings */
body {
    font-family: 'Arial', sans-serif;
    background-color: #121212; /* Toq rang fon */
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    color: white;
}

/* Container */
.container {
    background-color: #1f1f1f; /* Toq kulrang fon */
    padding: 40px;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
    width: 450px;
    text-align: center;
    animation: slideIn 1s ease-out;
}

/* Heading */
h1 {
    font-size: 2.5rem;
    color: #FFD700; /* Oltin rang */
    margin-bottom: 20px;
    animation: fadeIn 2s ease-out;
}

/* Textarea for input */
textarea {
    width: 100%;
    height: 150px;
    padding: 12px;
    margin-bottom: 20px;
    border: 1px solid #444;
    border-radius: 8px;
    background-color: #333;
    color: white;
    font-size: 1rem;
    resize: none;
    box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
    transition: all 0.3s ease-in-out;
}

textarea:focus {
    border-color: #FFD700;
    background-color: #444;
}

/* Controls (dropdowns and button) */
.controls {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}

select, button {
    padding: 12px;
    border-radius: 8px;
    font-size: 1rem;
    border: 1px solid #444;
    background-color: #333;
    color: white;
    cursor: pointer;
    transition: all 0.3s ease-in-out;
    width: 30%;
}

select:hover, button:hover {
    background-color: #FFD700; /* Hover state for select and button */
    color: #121212;
}

button {
    background-color: #4CAF50; /* Green button */
    color: white;
    width: 100%;
    border-radius: 8px;
}

button:hover {
    background-color: #45a049;
}

/* Status text */
#status {
    font-size: 1rem;
    color: #ddd;
    margin-top: 15px;
    animation: fadeIn 2s ease-out;
}

/* Animations */
@keyframes slideIn {
    from {
        transform: translateY(-50px);
        opacity: 0;
    }
    to {
        transform: translateY(0);
        opacity: 1;
    }
}

@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}






/* styles.css */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #f5f5f5;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    color: #333;
}

.container {
    text-align: center;
    background-color: #ffffff;
    padding: 40px;
    border-radius: 10px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    width: 400px;
}

h1 {
    font-size: 28px;
    color: #333;
    margin-bottom: 20px;
}

.stt-box {
    margin: 20px 0;
}

button {
    background-color: #4CAF50;
    color: white;
    border: none;
    padding: 15px 30px;
    font-size: 18px;
    cursor: pointer;
    border-radius: 5px;
    margin: 10px;
    transition: background-color 0.3s;
}

button:disabled {
    background-color: #ccc;
    cursor: not-allowed;
}

button:hover {
    background-color: #45a049;
}

.output {
    margin-top: 30px;
}

#text-output {
    font-size: 20px;
    color: #444;
    background-color: #e9e9e9;
    padding: 15px;
    border-radius: 5px;
    min-height: 50px;
    word-wrap: break-word;
}


// app.js
document.getElementById('start-btn').addEventListener('click', startRecognition);
document.getElementById('stop-btn').addEventListener('click', stopRecognition);

let recognition;
let isRecognizing = false;

// Web Speech API'ni qo'llab-quvvatlovchi brauzerlar uchun
if ('webkitSpeechRecognition' in window || 'SpeechRecognition' in window) {
    recognition = new (window.SpeechRecognition || window.webkitSpeechRecognition)();
    recognition.lang = 'uz-UZ';  // O'zbek tilini tanlash
    recognition.interimResults = true; // Yordamchi natijalar
    recognition.continuous = true; // Bir vaqtning o'zida bir nechta qatorlarni tanish

    recognition.onstart = () => {
        isRecognizing = true;
        document.getElementById('start-btn').disabled = true;
        document.getElementById('stop-btn').disabled = false;
    };

    recognition.onend = () => {
        isRecognizing = false;
        document.getElementById('start-btn').disabled = false;
        document.getElementById('stop-btn').disabled = true;
    };

    recognition.onresult = (event) => {
        let transcript = '';
        for (let i = event.resultIndex; i < event.results.length; i++) {
            transcript += event.results[i][0].transcript;
        }
        document.getElementById('text-output').textContent = transcript;
    };

    recognition.onerror = (event) => {
        console.error('Ovozli matnni tanishda xatolik yuz berdi:', event.error);
    };
} else {
    alert('Sizning brauzeringizda Web Speech API mavjud emas. Iltimos, Google Chrome yoki Opera-dan foydalaning.');
}

function startRecognition() {
    recognition.start(); // Ovozli tanishni boshlash
}

function stopRecognition() {
    recognition.stop();  // Ovozli tanishni to'xtatish
}





const speakBtn = document.getElementById('speak-btn');
const textInput = document.getElementById('text-input');
const voiceSelect = document.getElementById('voice-select');
const rateSelect = document.getElementById('rate-select');
const pitchSelect = document.getElementById('pitch-select');
const statusText = document.getElementById('status');

let voices = [];
let speechSynthesis = window.speechSynthesis;

// Ovozlarni olish va ro'yxatga joylash
function loadVoices() {
    voices = speechSynthesis.getVoices();
    voiceSelect.innerHTML = ''; // Ro'yxatni tozalash
    voices.forEach(voice => {
        let option = document.createElement('option');
        option.textContent = voice.name + ' (' + voice.lang + ')';
        option.value = voice.name;
        voiceSelect.appendChild(option);
    });
}

// Ovozli xabarni aytish
function speakText() {
    const text = textInput.value.trim();
    if (!text) {
        statusText.textContent = 'Iltimos, matn kiriting!';
        return;
    }

    const utterance = new SpeechSynthesisUtterance(text);
    const selectedVoice = voiceSelect.value;
    const selectedRate = parseFloat(rateSelect.value);
    const selectedPitch = parseFloat(pitchSelect.value);

    const voice = voices.find(voice => voice.name === selectedVoice);
    if (voice) {
        utterance.voice = voice;
    }
    utterance.rate = selectedRate;
    utterance.pitch = selectedPitch;

    speechSynthesis.speak(utterance);
    statusText.textContent = 'Ovoz chiqarilmoqda...';
}

// Yangi ovozlar yuklanadi
if (speechSynthesis.onvoiceschanged !== undefined) {
    speechSynthesis.onvoiceschanged = loadVoices;
}

// Boshqa o'zgarishlarni amalga oshirish
speakBtn.addEventListener('click', speakText);

// Dastlabki ovozlar yuklanadi
loadVoices();
