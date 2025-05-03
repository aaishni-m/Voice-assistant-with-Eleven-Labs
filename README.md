Personalized Voice Assistant with ElevenLabs

This project demonstrates how to build a personalized voice assistant using the ElevenLabs API. The assistant is configured to interact with users in real-time, providing responses based on a predefined schedule and context.

---

Features
- Personalized Responses: Customize the assistant's name, schedule, and context.
- Voice Interaction: Real-time audio input and output.
- Secure Credentials: Use environment variables to store sensitive information.
- Callback Functions: Monitor and log user-agent interactions.

---

Setup

Prerequisites
1. Python 3.8 or higher
2. Pip: Ensure it’s installed (`pip --version`).
3. ElevenLabs API Access:
   - Sign up at [ElevenLabs](https://www.elevenlabs.io).
   - Create an API key and Agent ID.

Clone the Repository
```bash
git clone https://github.com/your-repo-name/personalized-voice-assistant.git
cd personalized-voice-assistant
```

Install Dependencies
1. Install `pip` packages:
   ```bash
   pip install elevenlabs python-dotenv
   ```

2. Update `pip` if required:
   ```bash
   pip install --upgrade pip
   ```

---

Configuration

Environment Variables
1. Create a `.env` file at the root of your project:
   ```bash
   touch .env
   ```

2. Add your API credentials to `.env`:
   ```env
   AGENT_ID=your_agent_id
   API_KEY=your_api_key
   ```

---

Usage

Run the Script
1. Start the script:
   ```bash
   python voice_assistant.py
   ```

2. Upon running, the assistant will greet you based on the predefined schedule:
   - Example: "Hello Aaishni, how can I help you today?"

Customize the Assistant
- Edit the following variables in `voice_assistant.py`:
  - User Name: Set the `user_name` variable.
  - Schedule: Update the `schedule` variable to reflect the user’s schedule.
  - Prompt: Modify the `prompt` variable to adjust the assistant’s behavior.

---

File Structure

```
personalized-voice-assistant/
│
├── .env                     # Environment variables file
├── voice_assistant.py       # Main script
├── README.md                # Documentation
└── requirements.txt         # Dependencies (optional)
```

---

Callback Functions
The script includes logging for interactions:
- Agent Response: Logs the assistant’s response.
- Interrupted Response: Logs truncated responses due to interruptions.
- User Transcript: Logs what the user says during interactions.

---

Troubleshooting
1. Environment Variables Not Loaded:
   - Ensure `.env` is in the root directory.
   - Verify no spaces around `=` in `.env`.

2. Module Not Found:
   - Install missing modules:
     ```bash
     pip install <module-name>
     ```

3. Audio Interface Errors:
   - Check microphone and speaker permissions on your system.

---

Future Enhancement
- Add dynamic scheduling using an external calendar API.
- Enable conversation history for better context retention.
- Integrate text-based chat alongside voice interaction.

---

Credits
Developed using the [ElevenLabs API](https://www.elevenlabs.io).
