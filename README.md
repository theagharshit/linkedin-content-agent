# Linkedin-Content-Agent

What this does

Automates the creation of high-quality LinkedIn posts and visuals using LLMs, with a built-in human approval step before publishing.

Why this exists

Creating consistent, insight-driven LinkedIn content is time-consuming and repetitive. This system reduces manual effort while retaining editorial control through human-in-the-loop review and feedback.

How it works (high-level)
	1.	A webhook triggers post generation with a topic and target audience
	2.	An LLM generates the post copy and an image prompt
	3.	An AI-generated image is created and stored
	4.	The content is emailed for approval or feedback
	5.	Feedback triggers regeneration when required
	6.	Post status and assets are tracked in Google Sheets and Drive

Tech stack
	•	LLMs (text + image generation)
	•	n8n for workflow orchestration
	•	Webhooks for event-driven execution
	•	Google Sheets & Drive for state and asset management
