# ModernChatterBot

> A modern, AI-powered Discord bot with advanced web search capabilities using the Tavily API, built with Python and [discord.py](https://discordpy.readthedocs.io/). Ideal for interactive Discord communities.

![ModernChatterBot Banner](https://repository-image-url/placeholder.png) <!-- Replace with actual banner URL if you have one -->

---

## 🌟 Features

### 🔍 Web Search with Tavily  
Use the `/search` slash command with configurable depth options:  
- **Basic**: Quick searches  
- **Advanced**: Deep analysis with AI summaries  

### 🧠 AI Chat Support  
Interact with AI models such as **Groq**, **OpenAI**, or **Claude** using `/chat`.

### ⚠️ Enhanced Error Handling  
Smart retry logic for rate limits, timeouts, and API errors with detailed logging.

### 🧾 Clean Output  
Beautifully formatted Discord embeds with:
- Titles
- Snippets
- Direct links
- AI-generated summaries

### ⚙️ Flexible Configuration  
Customize settings like:
- Preferred AI provider
- Token limit
- Chat memory
- Image inclusion
- Search domains

### 🛡️ Content Filtering  
Ensures queries and responses remain safe and appropriate for Discord.

### 🧪 Debug Mode  
Use `debug.py` to test API integrations.

---

## 🔧 Prerequisites

- Python 3.8+
- [Discord Bot Token](https://discord.com/developers/applications)
- [Tavily API Key](https://tavily.com/)
- (Optional) API key from Groq, OpenAI, or Claude

---

## 📦 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/saurav714/ModernChatBot-main.git
cd ModernChatBot-main
2. Install Dependencies
bash
Copy
Edit
pip install discord.py python-dotenv aiohttp langchain langchain-community sentence-transformers
3. Set Environment Variables
Create a .env file in the root:

ini
Copy
Edit
# Required
DISCORD_PASS_KEY=your_discord_bot_token_here
TAVILY_API_KEY=your_tavily_api_key
GROQ_API_KEY=your_groq_api_key  # Or use OPENAI_API_KEY or CLAUDE_API_KEY

# Optional
AI_PROVIDER=groq
AI_TEMPERATURE=0.7
AI_MAX_TOKENS=1024
AI_RETRIES=3
TAVILY_MAX_RESULTS=5
MAX_CHAT_HISTORY=20
SIMILARITY_THRESHOLD=0.65
MEMORY_CLEANUP_INTERVAL=3600
INACTIVE_CHANNEL_TIMEOUT=86400
MAX_MESSAGE_LENGTH=1900
CHROMA_PERSIST_DIR=./chroma_db
🤖 Invite the Bot to Your Server
Go to the Discord Developer Portal

Select your bot → Bot tab → Copy token

Navigate to OAuth2 → URL Generator:

Scopes: bot, applications.commands

Bot Permissions: Send Messages, Embed Links, Read Message History

Use the generated URL to invite your bot to your server

🚀 Usage
To start the bot:

bash
Copy
Edit
python bot.py
Once running, it will:

Log in to Discord

Sync slash commands

Be ready for interaction

📚 Slash Commands
Command	Description
/search	Web search using Tavily API
/chat	Chat with AI (Groq/OpenAI/Claude/etc.)
/preferences	Customize your AI preferences
/stats	View bot stats
/clear	Clear chat history
/help	Display help info

Example
bash
Copy
Edit
/search query:"latest AI news" depth:advanced
📈 Logging
Logs are stored in bot.log, including:

Timestamps

Search success/failure

API errors and retries

🤝 Contributing
Fork the repository

Create a new branch:

bash
Copy
Edit
git checkout -b feature/YourFeature
Commit your changes:

bash
Copy
Edit
git commit -m "Add YourFeature"
Push and open a PR

📜 License
This project is licensed under the MIT License.

📬 Contact
GitHub Issues: Open here

Discord: saurav1099

Built with ❤️ by Saurav — Arise, Tarnished Warrior!
Created on June 08, 2025
