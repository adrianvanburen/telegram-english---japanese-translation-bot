# telegram-english---japanese-translation-bot
A simple python bot that automatically translates between Japanese and English in telegram chat rooms.

Edit bot.py to include your bot's token, obtained from telegram's @botfather special account:
https://core.telegram.org/bots/features#botfather

Install dependancies:
pip install easygoogletranslate python-telegram-bot --upgrade

Run:
python3 bot.py

You can set it up as a daemon or run in screen.

Please note, this bot uses a hack to access google's translation service without using their cloud API. It works by sending a carefully-crafted ajax request to google.com/translate and returns the result. If google makes changes to their website, this bot will break. This means your translation is limited to 5000 characters and subject to unknowable rate limits. So do use it for your personal life, but don't use it for business or critical things.
