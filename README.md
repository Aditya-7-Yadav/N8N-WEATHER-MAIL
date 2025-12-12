<div align="center">
🌤️ Gmail Weather – Automated Daily Email (n8n Workflow)

Get your daily Nagpur weather report delivered straight to your Gmail every morning.

🔁 Powered by n8n • ☁ OpenWeatherMap • ✉ Gmail OAuth
</div>
✨ What This Workflow Does

⏰ Runs every day at 6:00 AM

🌦 Fetches live weather from OpenWeatherMap

📧 Sends a formatted weather update email through Gmail

🔒 Keeps all API keys & tokens secure inside n8n (not in the repo)

🧩 Workflow Breakdown
1️⃣ Schedule Trigger

Triggers the workflow every morning at 06:00 AM.

2️⃣ OpenWeatherMap Node

Fetches weather for:

📍 City: Nagpur

Requires an OpenWeatherMap API Credential (you add this inside n8n).

3️⃣ Gmail Node

Sends an email containing:

Hey Bro!
Today's weather-
Max: {{ temp_max }}
Min: {{ temp_min }}
Description: {{ description }}


All values are dynamically inserted from the API response.

📥 Importing the Workflow

Open n8n

Navigate to Workflows → Import

Select the gmail-weather.json file

Set your credentials:

🔑 OpenWeatherMap API

✉ Gmail OAuth2

📁 Files Included
File	Purpose
gmail-weather.json	Main exported n8n workflow
🧰 Customization Options

You can modify any of the following in seconds:

🏙️ City name

🕒 Trigger time

✉ Recipient email

🧾 Email message style

🌡 Extra weather fields (humidity, wind, etc.)

🔐 Security Notice

No credentials, API keys, or sensitive info are stored in this repository.
n8n keeps all secrets encrypted on your local setup.

📄 License

Free for personal, educational, and experimental use.
Feel free to fork, modify, or extend!

<div align="center">

</div>
