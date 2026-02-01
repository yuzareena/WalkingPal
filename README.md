# 🎙️ WalkingPal

**Voice Companions for Meaningful Conversations**

A beautiful web interface for conversing with ElevenLabs AI voice agents. Choose between a supportive Friend or caring Parent companion, and communicate through voice or text.

---

## ✨ Features

- 🎨 **Elegant Design** - Stunning gradient interface with smooth animations
- 👥 **Two AI Companions** - Friend agent for casual chat, Parent agent for guidance
- 🎤 **Voice Input** - Speak naturally through your microphone
- ⌨️ **Text Input** - Type messages when you prefer (agent still responds with voice!)
- 🔄 **Dual Mode** - Seamlessly switch between voice and text
- 💫 **Real-time Feedback** - Visual indicators show when agent is speaking/listening
- 💾 **Auto-Save Settings** - Your configuration saves locally in browser
- 🔗 **Persistent Connection** - Long conversations without disconnection

---

## 🚀 Live Demo

**Visit:** [https://yuzareena.github.io/WalkingPal/](https://yuzareena.github.io/WalkingPal/)

---

## 🎯 Quick Start

### 1. **Get Your Agent IDs**
   - Go to [ElevenLabs](https://elevenlabs.io) and create two conversational AI agents
   - One for "Friend" personality
   - One for "Parent" personality
   - Copy their Agent IDs

### 2. **Open WalkingPal**
   - Visit the live site
   - Scroll to the Configuration section

### 3. **Enter Your Credentials**
   ```
   Friend Agent ID: [Your friend agent ID]
   Parent Agent ID: [Your parent agent ID]
   API Key: [Optional - only for private agents]
   ```

### 4. **Start Talking!**
   - Choose Friend or Parent
   - Click "Start Conversation"
   - Allow microphone access
   - Wait for agent greeting
   - Speak or type your messages

---

## 🔧 Configuration

### For Public Demo (Optional)

If you want to share your agents publicly, you can pre-fill the configuration in the HTML file:

**⚠️ SECURITY WARNING:** Never commit your API key to a public repository!

Edit the `index.html` file and update these lines (around line 380):

```javascript
// For demo purposes only - use public agents without API key
const savedFriendId = 'YOUR_FRIEND_AGENT_ID_HERE';
const savedParentId = 'YOUR_PARENT_AGENT_ID_HERE';
// DO NOT include API key in public repos
```

### Private Use

Keep the configuration section empty and let users enter their own credentials. Settings are saved locally in their browser.

---

## 💬 How It Works

### Agent Selection
- **Friend Mode** 🟢 - Casual conversations, brainstorming, companionship
- **Parent Mode** 🔴 - Guidance, advice, supportive wisdom

### Communication Methods

**Voice Input:**
- Speak naturally into your microphone
- Agent transcribes and responds with voice
- Perfect for hands-free conversation

**Text Input:**
- Type messages in the chat box
- Press Enter or click Send
- Agent still responds with voice
- Great for quiet environments

---

## 🛠️ Technical Details

### Built With
- Pure HTML/CSS/JavaScript (no frameworks needed)
- ElevenLabs Conversational AI API
- WebSocket for real-time communication
- Web Audio API for voice processing

### Browser Support
- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari
- ⚠️ Requires HTTPS for microphone access

### Audio Format
- Input: PCM 16000 Hz mono
- Output: PCM 16000 Hz mono
- Real-time streaming via WebSocket

---

## 📱 Usage Examples

### Scenario 1: Commute Companion
"I'm driving home and need someone to talk to about my day."
- Select **Friend** agent
- Use **Voice** input
- Have a natural conversation hands-free

### Scenario 2: Work Break
"I'm at the office and need quick advice but can't talk out loud."
- Select **Parent** agent  
- Use **Text** input (type questions)
- Listen to voice responses through headphones

### Scenario 3: Evening Chat
"I want to brainstorm some ideas before bed."
- Select **Friend** agent
- Mix **Voice** and **Text** as needed
- Switch between modes naturally

---

## 🎨 Customization

### Change Colors
Edit CSS variables in `index.html` (around line 20):

```css
:root {
    --accent-friend: #00f5d4;  /* Friend agent color */
    --accent-parent: #ff6b9d;  /* Parent agent color */
    --bg-dark: #0a0e1a;        /* Background */
}
```

### Modify Agent Descriptions
Update the `agentData` object in JavaScript (around line 280):

```javascript
const agentData = {
    friend: {
        name: 'Your Custom Name',
        description: 'Your custom description'
    }
};
```

---

## 🔒 Privacy & Security

- ✅ All credentials stored locally in browser
- ✅ No data sent to third parties (only ElevenLabs)
- ✅ Audio processed in real-time (not recorded)
- ✅ Clear all data by clearing browser storage
- ⚠️ Never share your API key publicly
- ⚠️ Use public agents for demos only

---

## 🐛 Troubleshooting

### "Invalid message received" error
- Check that Agent IDs are correct
- Verify agents are properly configured in ElevenLabs
- Try regenerating your API key

### Microphone not working
- Ensure browser has microphone permissions
- Check system audio settings
- Try using HTTPS (required for mic access)

### Agent disconnects quickly
- Check your internet connection
- Verify Agent IDs are active
- Try refreshing the page

### No audio from agent
- Check browser audio permissions
- Verify system volume is up
- Try a different browser

---

## 📄 License

This project is open source and available for personal and educational use.

---

## 🙏 Acknowledgments

- **ElevenLabs** - For amazing conversational AI technology
- **Design Inspiration** - Modern glassmorphism and gradient trends
- **Fonts** - Playfair Display & DM Sans from Google Fonts

---

## 📞 Support

Have questions or issues?
- Open an issue on this repository
- Check ElevenLabs documentation: [docs.elevenlabs.io](https://docs.elevenlabs.io)

---

## 🚀 Future Enhancements

- [ ] Multiple agent personalities
- [ ] Conversation history
- [ ] Voice selection per agent
- [ ] Custom agent avatars
- [ ] Mobile app version
- [ ] Conversation export

---

**Made with ❤️ for meaningful AI conversations**

⭐ Star this repo if you find it useful!
