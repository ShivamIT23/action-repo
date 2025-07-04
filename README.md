# Action Repo — GitHub Webhook Trigger

This repository is used to trigger webhook events for the [Webhook Receiver App](https://github.com/ShivamIT23/tsk-public-assignment-webhook-repo).

Whenever you:
- Push a commit
- Create a pull request
- Merge a pull request

➡️ GitHub will send a webhook event to the registered endpoint.

---

## 🔗 Webhook Configuration

This repository has a GitHub Webhook configured to send events to:

POST [https://tsk-public-assignment-webhook-repo-jeh7.onrender.com/webhook](https://tsk-public-assignment-webhook-repo-jeh7.onrender.com/webhook)

It is triggered on:
- Push events
- Pull request events (opened, closed/merged)

---

## 🧪 How to Test

1. Clone the repo
2. Make any commit and push it:
   ```bash
   git commit -m "Test push"
   git push
   ```
3. Create a pull request on GitHub

4. Merge that pull request

Each of these actions will send a JSON payload to the webhook receiver and get stored in MongoDB Atlas via the Flask app.

📦 Connected Repositories
Webhook Receiver App: [WebHook-repo](https://github.com/ShivamIT23/tsk-public-assignment-webhook-repo)

Live UI: [Link](https://tsk-public-assignment-webhook-repo-jeh7.onrender.com/)
