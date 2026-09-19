# Tsum Discord Bot

`bot.py` is the entry point. It loads `.env`, registers the persistent Discord views, and syncs slash commands.

## Setup

1. Install Python 3.11+.
2. Run `pip install -r requirements.txt`.
3. Copy `.env.example` to `.env`.
4. Fill in `TOKEN`, `SERVER_ID`, `OWNER_ID`, and optionally `LOG_CHANNEL_ID`.
5. Start with `python bot.py`.

## Files

- `bot.py` — Discord bot entry point and slash commands.
- `mod_stum.py` — Discord UI, login flow, menu execution, free-use tracking.
- `api2.py` — LINE/Tsum API client and game operations.

## Important

Do not commit `.env` or real login credentials/tokens to a public repository. The bot expects the LINE login flow and API endpoints used by the supplied source to remain valid.

`free_users.json` is created automatically when the one-time trial is used.
