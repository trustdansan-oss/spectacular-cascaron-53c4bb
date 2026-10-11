FAST — Direct Gmail Email Setup

This package keeps the existing tracking pages and adds a Netlify Function for direct Gmail sending.

IMPORTANT
- Do not put your Gmail App Password in any HTML/JavaScript file. It belongs only in Netlify environment variables.
- Netlify environment variables required: GMAIL_USER (your full Gmail address), GMAIL_APP_PASSWORD (the Gmail App Password).
- After adding or changing environment variables, deploy the site again.

DEPLOY
1. Download and extract this ZIP.
2. Upload the extracted site folder contents to your existing Netlify site's manual deploy area, including index.html, fast.html, public/, package.json, and netlify/. Do not upload only the HTML files; the netlify/functions/send-email.mjs function is required.
3. Wait for the deploy to finish.
4. Open the website, choose a shipment's email preview, check the recipient, edit the message if needed, and tap “Send email directly”.
5. Test first with an email address you control.

If the page opens but sending fails, open Netlify > Functions and check send-email logs. Make sure the environment variables are set for the deploy context used by the published site.
