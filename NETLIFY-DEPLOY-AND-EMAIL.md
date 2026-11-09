# Bizware Solution — Netlify deployment and enquiry emails

## Deploy
1. Sign in to https://app.netlify.com/.
2. Use **Add new project / Add new site → Deploy manually** (wording may vary).
3. Extract this ZIP locally, then drag the **extracted folder** (containing index.html) into the Netlify deploy area.
4. Open the resulting *.netlify.app URL.

## Enable the contact form
1. On your new Netlify site, open **Forms**.
2. Enable **Form detection** if it is disabled, and **redeploy the extracted site**.
3. Confirm that the form named **bizware-enquiry** is detected.

## Send enquiries to Habib.Tarafder@pdipdi.com
1. Open **Forms → Submission notifications → Add notification → Email notification**.
2. Select the **bizware-enquiry** form.
3. Set the recipient to **Habib.Tarafder@pdipdi.com**.
4. Save, then submit a test enquiry from the public website.
5. Confirm both that the test is in **Forms → bizware-enquiry** and that the recipient received an email.

IMPORTANT (current Netlify requirement): Except on Enterprise or Legacy Business plans, notification recipients
must be active members of the Netlify team. If Netlify rejects that email, invite the mailbox
owner to your Netlify team and have them accept the invitation before trying again.
Use a dedicated Bizware email address later if preferred; the present address is **not shown publicly**.

The visitor's email goes into the 'email' field, which Netlify can use for Reply-To.
Netlify may apply spam filtering and form usage limits.

Notes: Netlify notification destinations cannot be set from public static HTML.
This package can receive form submissions once deployed and detected; the recipient must be configured in Netlify.
No deployment has been performed by ChatGPT. Never share Netlify credentials or tokens in public files.

References:
https://docs.netlify.com/manage/forms/setup/
https://docs.netlify.com/manage/forms/notifications/
