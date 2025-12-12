Gmail Weather – n8n Automation

This n8n workflow automatically fetches the daily weather for Nagpur and sends it to a Gmail inbox every morning.

Overview

This automation performs the following steps:

Triggers every day at 6:00 AM

Fetches weather data from OpenWeatherMap

Sends an email through Gmail containing:

Maximum temperature

Minimum temperature

Weather description

Workflow Components
1. Schedule Trigger

Runs daily at 6 AM and initiates the workflow.

2. OpenWeatherMap Node

Fetches weather details for the city Nagpur.
Requires an OpenWeatherMap API credential (not included in the repo).

3. Gmail Node

Sends the weather update email using Gmail OAuth2 credentials (not included).

Email Format

The email sent looks like:

Hey Bro!
Today's weather-
Max: {{ temp_max }}
Min: {{ temp_min }}
Description: {{ description }}


Dynamic values are inserted from the weather API response.

Credentials Notice

This repository does not include any sensitive information such as API keys or OAuth tokens.
You must configure all credentials manually inside your n8n instance.

Import Instructions

Open n8n

Go to Workflows → Import

Upload the .json file from this repository

Assign your own credentials for:

OpenWeatherMap API

Gmail OAuth2

Files in This Repository
File	Description
gmail-weather.json	Exported n8n workflow file
Customization

You can easily modify:

City name

Email content

Trigger schedule

Recipient email

Directly using the n8n UI after importing.

License

Open for personal or educational use. Modify and extend as needed with giving me due credits.
