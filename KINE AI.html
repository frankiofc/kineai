<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kine AI - Smart Assistant</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    :root {
      --primary-color: #4361ee;
      --secondary-color: #3f37c9;
      --user-color: #4cc9f0;
      --ai-color: #f72585;
      --bg-color: #f8f9fa;
      --text-color: #212529;
      --light-gray: #e9ecef;
      --dark-gray: #6c757d;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: var(--bg-color);
      color: var(--text-color);
      display: flex;
      flex-direction: column;
      height: 100vh;
      line-height: 1.6;
    }

    header {
      background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
      color: white;
      padding: 1rem;
      text-align: center;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
      position: relative;
      z-index: 10;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .header-content {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .logo {
      width: 30px;
      height: 30px;
    }

    #chat-container {
      flex: 1;
      padding: 1rem;
      overflow-y: auto;
      display: flex;
      flex-direction: column;
      background-color: white;
      background-image: radial-gradient(var(--light-gray) 1px, transparent 1px);
      background-size: 20px 20px;
    }

    .message {
      padding: 0.8rem 1.2rem;
      margin: 0.5rem 0;
      border-radius: 1.2rem;
      box-shadow: 0 3px 6px rgba(0,0,0,0.05);
      position: relative;
      transition: background 0.3s ease;
      display: flex;
      flex-direction: column;
      max-width: 80%;
    }

    .message.user {
      align-self: flex-end;
      background: linear-gradient(145deg, var(--user-color), #38bdf8);
      color: white;
      border-bottom-right-radius: 0.3rem;
    }

    .message.ai {
      align-self: flex-start;
      background: #f1f3f5;
      color: #111;
      border-bottom-left-radius: 0.3rem;
    }

    .timestamp {
      font-size: 0.7rem;
      color: var(--dark-gray);
      margin-top: 4px;
      align-self: flex-end;
    }

    .typing-indicator {
      display: flex;
      align-items: center;
      padding: 0.5rem 1rem;
      background: #f1f1f1;
      border-radius: 1rem;
      width: fit-content;
      max-width: 150px;
      margin: 0.5rem 0;
    }

    .typing-dot {
      width: 8px;
      height: 8px;
      background: #555;
      border-radius: 50%;
      margin: 0 2px;
      animation: blink 1.4s infinite ease-in-out both;
    }

    .typing-dot:nth-child(2) {
      animation-delay: 0.2s;
    }
    .typing-dot:nth-child(3) {
      animation-delay: 0.4s;
    }

    @keyframes blink {
      0%, 80%, 100% {
        transform: scale(0);
      } 
      40% {
        transform: scale(1);
      }
    }

    #input-container {
      display: flex;
      padding: 1rem;
      background-color: white;
      border-top: 1px solid var(--light-gray);
      box-shadow: 0 -2px 10px rgba(0,0,0,0.05);
    }

    #user-input {
      flex: 1;
      padding: 0.8rem 1rem;
      font-size: 1rem;
      border: 1px solid var(--light-gray);
      border-radius: 2rem;
      outline: none;
      transition: all 0.3s ease;
    }

    #user-input:focus {
      border-color: var(--primary-color);
      box-shadow: 0 0 0 2px rgba(67, 97, 238, 0.2);
    }

    #send-btn {
      padding: 0.8rem 1.5rem;
      margin-left: 0.8rem;
      font-size: 1rem;
      background-color: var(--primary-color);
      color: white;
      border: none;
      border-radius: 2rem;
      cursor: pointer;
      transition: all 0.3s ease;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    #send-btn:hover {
      background-color: var(--secondary-color);
      transform: translateY(-1px);
    }

    #send-btn:active {
      transform: translateY(0);
    }

    #reset-btn {
      padding: 0.8rem 1.5rem;
      font-size: 1rem;
      background-color: #e4e6eb;
      color: #333;
      border: none;
      border-radius: 2rem;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    #reset-btn:hover {
      background-color: #d0d3d4;
      transform: translateY(-1px);
    }

    #reset-btn:active {
      transform: translateY(0);
    }

    #product-btn {
      background-color: #f72585;
      color: white;
      border: none;
      border-radius: 2rem;
      padding: 0.7rem 1.2rem;
      font-size: 0.9rem;
      text-decoration: none;
      display: flex;
      align-items: center;
      gap: 0.5rem;
      transition: all 0.3s ease;
    }

    #product-btn:hover {
      background-color: #c9184a;
      transform: translateY(-1px);
    }

    @media (max-width: 768px) {
      .message {
        max-width: 90%;
      }
      
      #user-input {
        padding: 0.7rem 1rem;
      }
      
      #send-btn, #reset-btn, #product-btn {
        padding: 0.7rem 1.2rem;
        font-size: 0.85rem;
      }
    }

    @media (max-width: 480px) {
      header {
        padding: 0.8rem;
        flex-direction: column;
        gap: 0.5rem;
      }
      
      .message {
        max-width: 95%;
      }
      
      #input-container {
        padding: 0.8rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="header-content">
      <i class="fas fa-robot logo"></i>
      <h1>Kine AI</h1>
    </div>
    <div style="display: flex; gap: 0.5rem;">
      <a href="https://tinyurl.com/produkfranki" target="_blank" id="product-btn">
        <i class="fas fa-globe"></i> Produk Franki
      </a>
      <button id="reset-btn">
        <i class="fas fa-undo"></i> Reset
      </button>
    </div>
  </header>

  <div id="chat-container"></div>

  <div id="input-container">
    <input type="text" id="user-input" placeholder="Tanya sesuatu..." autocomplete="off" />
    <button id="send-btn">
      <i class="fas fa-paper-plane"></i>
      <span class="btn-text">Kirim</span>
    </button>
  </div>

  <script>
    const apiKey = "free1";

    const chatContainer = document.getElementById('chat-container');
    const userInput = document.getElementById('user-input');
    const sendBtn = document.getElementById('send-btn');
    const resetBtn = document.getElementById('reset-btn');

    function getCurrentTime() {
      const now = new Date();
      return now.toLocaleTimeString([], { hour: '2-digit', minute: '2-digit' });
    }

    function createTypingIndicator() {
      const indicator = document.createElement('div');
      indicator.classList.add('message', 'ai');
      indicator.innerHTML = `
        <div class="typing-indicator">
          <div class="typing-dot"></div>
          <div class="typing-dot"></div>
          <div class="typing-dot"></div>
        </div>
      `;
      return indicator;
    }

    function addMessage(text, sender) {
      const message = document.createElement('div');
      message.classList.add('message', sender);

      const messageContent = document.createElement('div');
      messageContent.textContent = text;
      message.appendChild(messageContent);

      const timestamp = document.createElement('div');
      timestamp.classList.add('timestamp');
      timestamp.textContent = getCurrentTime();
      message.appendChild(timestamp);

      chatContainer.appendChild(message);
      chatContainer.scrollTop = chatContainer.scrollHeight;
    }

    async function getKineAiResponse(prompt) {
      try {
        const encodedPrompt = encodeURIComponent(prompt);
        const response = await fetch(`https://api.ubed.my.id/ai/Gpt4o-turbo?apikey=${apiKey}&ask=${encodedPrompt}`);
        if (!response.ok) throw new Error(`HTTP error! status: ${response.status}`);
        const data = await response.json();
        return data.result || data.respon || "Maaf, tidak mendapat respons dari server.";
      } catch (error) {
        console.error("Error fetching AI response:", error);
        return `Error: Gagal menghubungi AI (${error.message})`;
      }
    }

    async function handleSend() {
      const text = userInput.value.trim();
      if (!text) return;

      addMessage(text, 'user');
      userInput.value = '';
      userInput.focus();

      const typingIndicator = createTypingIndicator();
      chatContainer.appendChild(typingIndicator);
      chatContainer.scrollTop = chatContainer.scrollHeight;

      try {
        const reply = await getKineAiResponse(text);
        setTimeout(() => {
          chatContainer.removeChild(typingIndicator);
          addMessage(reply, 'ai');
        }, 1000 + Math.random() * 1000);
      } catch (err) {
        chatContainer.removeChild(typingIndicator);
        addMessage("Gagal mendapatkan respons dari AI.", 'ai');
      }
    }

    async function handleReset() {
      chatContainer.innerHTML = '';
      addMessage("Hai! Saya Kine AI, asisten virtual Anda. Saya dikembangkan oleh Franki. Ada yang bisa saya bantu?", 'ai');
    }

    sendBtn.addEventListener('click', handleSend);
    userInput.addEventListener('keydown', (e) => {
      if (e.key === 'Enter') handleSend();
    });
    resetBtn.addEventListener('click', handleReset);

    setTimeout(() => {
      addMessage("Hai! Saya Kine AI, asisten virtual Anda. Saya dikembangkan oleh Franki. Ada yang bisa saya bantu?", 'ai');
    }, 500);
  </script>
</body>
</html>
