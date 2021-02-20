This is a basic server that handles Slack requests from Event Subscriptions of the ServerMessenger App in my Slack chat room. The network communication is handled through ngrok (`./ngrok http 3000`), which produces a different temporary URL at each run that needs to be entered in the app `Event Subscriptions` page (e.g. `http://467753713891.ngrok.io/slack/events`).

This server creates a home page for the ServerMessenger App and watches for messages that include "talk to me," which will trigger a basic text reply message.

This was created starting with the tutorial at https://api.slack.com/start/building/bolt-python
