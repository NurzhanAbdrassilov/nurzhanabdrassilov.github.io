---
title: "AIna – Your Intelligent Ally for an Accessible Web"
layout: single 
excerpt: "AIna is your AI-powered co-pilot for visual web accessibility—analyzing websites, grading compliance, and guiding improvements to build a safer, more inclusive internet for everyone. <br/><img src='/images/aina.png'>"
collection: projects
---

## Inspiration

Over 2.2 billion people globally live with a visual or cognitive disability, yet 96.3% of the top 1 million websites still fail basic accessibility checks (WebAIM, 2024). From low-contrast text and unlabeled elements to flashing visuals that can trigger seizures, accessibility is still an afterthought on most of the web.

We built Aina to change that — making web accessibility smarter, automated, and truly user-centered.

## What It Does

- 🧪 **Site Scanner** – Input any URL to trigger a deep scrape of the site’s code and layout  
- 🧠 **AI-Powered Analysis** – Uses Gemini Flash 2.0 to evaluate HTML, CSS, and visual components  
- 🧾 **Accessibility Grade** – Badge-based score out of 7, based on WCAG 2.1  
- 📋 **Detailed Feedback** – Actionable improvement tips from AI  
- 🗂 **Live Dashboard** – Public catalogue of scanned websites (stored in MongoDB Atlas)  
- ⚙️ **Accessible UI** – Toggleable high-contrast mode for demo accessibility  
- 🛡️ **Coming Soon** – Blockchain-based accessibility certificates  

## How We Built It

- **Frontend**: React + TypeScript  
- **Backend**: Node.js, Express, JSDOM  
- **Database**: MongoDB Atlas on AWS  
- **AI**: Gemini Flash 2.0 API  
- **Design**: Accessibility-first responsive interface with contrast/dark/light modes  

## Challenges We Ran Into

- Scraping inconsistent or bloated web structures  
- Designing an objective and interpretable scoring system  
- Getting consistent and helpful responses from Gemini  
- Blockchain integration introduced bugs (deferred for post-hackathon)

## Accomplishments

- 🚀 Built a full-stack AI accessibility platform in under 48 hours  
- 🤝 Integrated real-time Gemini accessibility audits  
- 📊 Developed a live public dashboard  
- 🎨 Shipped a fully accessible interface with contrast mode  

## What We Learned

- DOM parsing and scraping are real-world engineering challenges  
- How to prompt engineer Gemini effectively  
- Cloud database deployment with MongoDB Atlas  
- Accessibility must be intentional, not an afterthought  
- Costco pizza keeps you alive during crunch time

## What’s Next

- 🧬 Fine-tuned suggestions tailored for different roles (developer, designer, user)  
- 🔒 Blockchain-based certification for compliant websites  
- 👥 User testing with assistive tech communities  
- 🌍 Browser extension for real-time scans  
- 📢 Developer advocacy through accessibility awareness

## Links

- 🔗 [Live Demo](https://caneyeuseit.tech)  
- 💻 [GitHub Repo](https://github.com/nurzhanabdrassilov/aina)