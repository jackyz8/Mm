FIXED HOSTING BOT

1. Replace your old app.py with this app.py.
2. Keep your own .env on the hosting panel; do NOT upload/share it publicly.
3. Install packages: pip install -r requirements.txt
4. Restart the bot.

Fix: CPU usage collection now catches PermissionError/OSError/psutil errors when the host blocks /proc/stat, so status screens can fall back to 0% CPU instead of failing. This addresses the screenshot error path; other unrelated errors may still need separate fixes.

Security: if your bot token was ever shared in a screenshot/chat/archive, revoke it via BotFather and set the new token in your private environment.
