# 🍑 GA Peach AI Twin

**Create AI-generated images of your custom “Peach” avatar directly from your prompt.** Built with OpenAI + Google Cloud Functions.

---

## 🌟 Live App
👉 [Use the GA Peach AI Twin](https://us-central1-silken-phalanx-483504-v2.cloudfunctions.net/gaPeachGenerate3)

---

## 🚀 Features
- Generate custom AI Peach avatars
- OpenAI DALL·E backend
- Hosted on Google Cloud Functions
- BYOK (Bring Your Own Key) ready
- API & browser ready

---

## 🔧 Tech Stack
- **Frontend**: Linktree (external wrapper) or Web page
- **Backend**: Node.js 22, Google Cloud Functions
- **AI Model**: OpenAI DALL·E 3 (via `images/generations` endpoint)
- **Auth**: API Key (environment variable)

---

## 📦 Installation (for Devs)
Clone and deploy with Google Cloud:

```bash
git clone https://github.com/yourusername/ga-peach-ai-twin.git
cd ga-peach-ai-twin
gcloud functions deploy gaPeachGenerate3 \
  --entry-point=generate \
  --runtime=nodejs22 \
  --trigger-http \
  --allow-unauthenticated \
  --source=.

