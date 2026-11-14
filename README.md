# JONATHAN-MD

A small starter bot using the **official WhatsApp Cloud API**. It replies to incoming text messages and supports `!help` and `!about`.

## Important
- This is starter code, not a bot that is already online.
- It requires a Meta developer app, WhatsApp Cloud API setup, and a public HTTPS webhook.
- Use only the official API. Do not scan QR codes on unknown bot sites or share WhatsApp pairing codes.
- Keep access tokens and `.env` private. Never commit `.env` to GitHub.
- The Cloud API has messaging rules, including the customer-service window and approved templates for some business-initiated messages.

## Run locally
1. Install a current Node.js release.
2. Run `npm install`.
3. Copy `.env.example` to `.env` and fill in your Meta credentials.
4. Run `npm start`.

A local server is not publicly reachable by Meta. For real webhook testing, deploy it to a trusted HTTPS hosting service and configure that URL plus `/webhook` in your Meta app.

## Meta setup
Follow Meta's official WhatsApp Cloud API documentation:
https://developers.facebook.com/docs/whatsapp/cloud-api/

Set the webhook verify token to the same value as `VERIFY_TOKEN`, subscribe to the `messages` webhook field, and configure the app's WhatsApp phone number ID and access token as environment variables.

## GitHub
Upload `server.js`, `package.json`, `.gitignore`, `.env.example`, and `README.md` to a repository. Do **not** upload `.env`.
