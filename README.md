<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HealthTech-1 Chatbot Demo</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            padding: 20px;
            background-color: #f8f9fa;
            color: #333;
        }

 /* Floating Chatbot Button */
        .chatbot-button {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #4A90E2;
            color: white;
            border: none;
            padding: 15px;
            border-radius: 50%;
            cursor: pointer;
            font-size: 18px;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2);
        }

/* Chatbot Container */
        .chatbot-container {
            position: fixed;
            bottom: 80px;
            right: 20px;
            width: 350px;
            height: 500px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2);
            display: none;
            flex-direction: column;
            border: 1px solid #ddd;
        }

 /* Chatbot Header */
        .chatbot-header {
            background-color: #4A90E2;
            color: white;
            padding: 10px;
            font-size: 16px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-top-left-radius: 10px;
            border-top-right-radius: 10px;
        }

 .minimize-button {
            background: none;
            border: none;
            color: white;
            font-size: 22px;
            cursor: pointer;
        }

 /* Chatbot Iframe */
        .chatbot-iframe {
            width: 100%;
            height: 100%;
            border: none;
        }
    </style>
</head>
<body>

<h1 style="color: #0056b3;">HealthTech-1 Chatbot Demo</h1>
    <p>Welcome! This is a demo chatbot showcasing how AI can assist HealthTech-1.</p>
 <!-- Chatbot Button -->
    <button class="chatbot-button" onclick="toggleChatbot()">💬</button>
 <!-- Chatbot Box -->
    <div class="chatbot-container" id="chatbotBox">
        <div class="chatbot-header">
            Chat Support
            <button class="minimize-button" onclick="toggleChatbot()">–</button>
        </div>
        <iframe class="chatbot-iframe"
            src="https://console.dialogflow.com/api-client/demo/embedded/2ba4a88b-2d90-4ac6-90b9-f195f09c4f52">
        </iframe>
    </div>

<p>Try asking about HealthTech-1 services, careers, and more!</p>

<script>
        function toggleChatbot() {
            var chatbot = document.getElementById("chatbotBox");
            chatbot.style.display = chatbot.style.display === "none" || chatbot.style.display === "" ? "flex" : "none";
        }
    </script>

</body>
</html>

