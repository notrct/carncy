from telegram import Update
from telegram.ext import Updater, CommandHandler, CallbackContext
import requests

TOKEN = "8582014244:AAGeZe0W1gG7YWUeKGYnOO09US9ObrgRMLA"

# ستاسو دوه اړین چینلونه
CHANNELS = ["@ProTech43", "@Pro43Zone"]

# نرخونو ویب لینک
PRICE_URL = "https://CG-zCGhLphP5hyWaz8nKRn33HC9"  # ستاسو لینک

def get_prices():
    # که لینک د JSON یا ساده متن API وي
    response = requests.get(PRICE_URL)
    if response.status_code == 200:
        return response.text
    else:
        return "نرخونه نشي ترلاسه کېدی."

def start(update: Update, context: CallbackContext):
    user_id = update.message.from_user.id
    # د ګډون چک کول
    for channel in CHANNELS:
        member = context.bot.get_chat_member(chat_id=channel, user_id=user_id)
        if member.status not in ["member", "creator", "administrator"]:
            update.message.reply_text(
                f"مهرباني وکړئ لومړی دې چینل ته جاین شئ: {channel}"
            )
            return

    # که دواړه چینلونه شامل وي
    update.message.reply_text("ټولو اړینو چینلونو ته جاین شو. اوس نرخونه:")
    update.message.reply_text(get_prices())

def main():
    updater = Updater(TOKEN)
    dp = updater.dispatcher
    dp.add_handler(CommandHandler("start", start))
    updater.start_polling()
    updater.idle()

if __name__ == "__main__":
    main() 
