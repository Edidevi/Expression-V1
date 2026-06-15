# 🧠 Expression V1

> A serverless, AI-powered mental well-being application that combines facial expression detection with personalised journaling to deliver compassionate, real-time mental health guidance. **NOT DESIGNED TO REPLACE THERAPY OR COUNSELLING, TO BE SEEN AS SELF STUDY**

**Live Demo:** [https://dc2b8er08430l.cloudfront.net/)
**Repository:** [https://github.com/Edidevi/Expression](

---

## 📖 Overview
<img width="305" height="303" alt="image" src="https://github.com/user-attachments/assets/73985d78-a945-4e96-aa47-242caf53e07f" />

Expression is a mental health journaling app built on AWS that meets users wherever they are — whether they check in daily or only reach out when they an outlet for extreme emotions. Users can log how they're feeling through written input and detected facial expressions. The app then uses AI to deliver personalised, empathetic well-being advice grounded in their actual emotional state.

The core insight behind the project: not everyone can fully label their own emotions. Emotional intelligence can be taught and learned — and this app helps bridge that gap through gentle, AI-guided reflection.


---

## ✨ Features

- **Mood Journaling** — Users describe how they're feeling in text; entries are stored per user with timestamps.
- **Facial Expression Detection** — Integrates with Amazon Rekognition to detect visual emotional cues.
- **AI-Powered Advice** — Uses Amazon Bedrock (Claude Haiku) to generate compassionate, 2-sentence therapeutic guidance tailored to each user's mood, expression data, and journal text.
- **User Authentication** — Secure sign-up and login via Amazon Cognito (email-based, JWT-authenticated).
- **Journal History** — Past entries are retrieved and displayed per authenticated user from DynamoDB.
- **Fully Serverless** — No servers to manage; the entire backend runs on AWS Lambda, API Gateway, and CloudFront.

---

## 💡 Design Decisions

**Why personalised AI advice rather than static content?**
Mental health is not one-size-fits-all. What works for one person may not help another. By combining the user's own written description with their detected visual expression, the AI can tailor advice to their specific state at that moment — making the app useful whether someone checks in every day or only when they're struggling.

**Why facial expression detection?**
Not everyone can fully articulate why they feel a certain way. Emotional intelligence is a learned skill, and the app uses Rekognition to surface cues the user may not have consciously registered, giving the AI more context for a more accurate and helpful response. Use of this tool coupled with counselling and therapeutic assistance, this could increase ones emotional intelligence.

**Why serverless?**
The fully serverless architecture (Lambda + API Gateway + DynamoDB + CloudFront) means zero infrastructure management, automatic scaling, and pay-per-request pricing — ideal for a wellness app with variable usage patterns.


