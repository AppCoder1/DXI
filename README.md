# DXI

This repository contains a minimal example of how to set up a LiveKit voice
agent in Python. The agent, named **John**, connects to Twilio to receive
inbound phone calls. It uses the `gpt-4.1-mini` model for language
understanding, ElevenLabs for text-to-speech (TTS), and Deepgram for
speech-to-text (STT).

## Requirements
- Python 3.10+
- `livekit-agents` Python package
- `twilio` SDK

## Environment variables
The following environment variables must be configured before running the
agent:

- `ELEVENLABS_API_KEY`
- `DEEPGRAM_API_KEY`
- `TWILIO_ACCOUNT_SID`
- `TWILIO_AUTH_TOKEN`
- `TWILIO_PHONE_NUMBER`

## Running the example
Install the required dependencies and run `voice_agent.py`:

```bash
python voice_agent.py
```

This will start the agent named John and await incoming calls via Twilio.
