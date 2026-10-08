# cutroom

Remove dead air from recordings, then auto-generate a recap article from the transcript.

## Features
- [x] Silence detection and removal (ffmpeg)
- [ ] Transcription (faster-whisper)
- [ ] Low-content segment flagging
- [ ] Cut list review (JSON) before rendering
- [ ] Recap article generation (Claude)

## Setup
brew install ffmpeg
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env

## Usage
python -m cutroom.main input/masterclass.mp4