# AI Image Generator Bot

A Telegram bot that generates images from text prompts using AI image services.

## Features
- Generate images with text prompts
- Supports custom width, height, and model options
- Uses `Pollinations.ai` first, then falls back to `Arta.ai`
- Sends the generated image back directly in Telegram
- Built with `pyTelegramBotAPI`

## Commands
- `/start` — welcome message and usage guide
- `/help` — same as `/start`
- `/admin` — bot creator information
- `/img` — generate an image

## Usage
Basic prompt:

```text
/img a cute cat wearing sunglasses
```

Custom size:

```text
/img 512 512 a futuristic robot in neon lights
```

Custom model:

```text
/img 1024 768 flux a cinematic city skyline at night
```

Format:

```text
/img [width] [height] [model] [prompt]
```

Supported model examples:
- `flux`
- `stable-diffusion`
- `dall-e`
- `glide`

## Setup
1. Install Python 3.10+.
2. Install dependencies:

```powershell
pip install -r requirements.txt
```

3. Add your Telegram bot token to `token.txt` in the project root.
4. Start the bot:

```powershell
python bot.py
```

## Project Structure
- `bot.py` — main bot logic
- `requirements.txt` — Python dependencies
- `token.txt` — local Telegram bot token file

## Notes
- The bot first tries `Pollinations.ai` for image generation.
- If that fails, it falls back to `Arta.ai`.
- Keep `token.txt` private and do not commit it to GitHub.

## Contributors
Created by Shrikant Bhama, Akash Singh, and Sajjan Singh.
