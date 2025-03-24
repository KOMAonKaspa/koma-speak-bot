# 🐶 Koma Speak Bot

**Talk to your dog. Get a reply. It’s KOMA magic.**

Ever wanted to say something to your dog?  
Now you finally can.  
Send a voice message — get a bark back.  
It’s fun, weirdly emotional, and just a little bit genius.

---

## ✨ Features

- 🎤 **Voice-to-Bark Translator** — you speak, your dog barks back (randomized)
- 🆓 **Free Tier** — 10 free barks per user
- 💰 **Subscription System** — 1 month (350 KAS), 6 months (1000 KAS)
- 🧠 **Smart User Tracking** — all bark counts stored in SQLite
- 🧾 **Manual Payment Approval** — users send TX hash, admin confirms
- 🎛️ **Admin Panel** — activate subscriptions via command
- 🐕 **Multiple Bark Files** — for wild, random barking behavior

---

## 🛠️ Setup

### 1. Clone this repo

```bash
git clone https://github.com/yourusername/koma-speak-bot.git
cd koma-speak-bot
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Install FFmpeg

Required for audio conversion with `pydub`.

```bash
# Ubuntu / Debian
sudo apt install ffmpeg

# Replit
apt update && apt install ffmpeg
```

---

## 🔧 Configuration

Open `main.py` and set the following:

```python
BOT_TOKEN = 'YOUR_TELEGRAM_BOT_TOKEN'
ADMIN_ID = 123456789   # Your Telegram numeric ID
KASPA_ADDRESS = 'kaspa:your_kaspa_wallet_address'
```

---

## 📁 Add Bark Files

Put your bark samples in the root folder:

```
bark.mp3
bark(1).mp3
bark(2).mp3
...
bark(9).mp3
```

The bot will randomly pick one for each voice response.

---

## 🚀 Run the bot

```bash
python3 main.py
```

---

## 👑 Admin Commands

To approve a user subscription:

```
/approve <user_id> <days>
```

Example:

```
/approve 123456789 30
```

---

## 🤖 Bot UI Preview

- `/start` — welcome + keyboard menu  
- 🔄 **Check Balance** — shows how many free barks left or subscription status  
- 💳 **Buy Subscription** — shows KASPA wallet + button "I Paid"  
- Users reply with TX hash, admin activates

---

## 🐾 Credit

Built by [@mrO00101](https://t.me/mrO00101)  
Powered by **Kaspa** blockchain love 💚

---

## 💡 Tip

Wanna go viral in crypto? Let your dog do the barking.
