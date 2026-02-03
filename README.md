📊 AI-Powered PowerPoint Generator

This project is a Python-based PowerPoint generator that uses Google Gemini AI to automatically create presentation content and Pexels to fetch relevant images.

It generates: AI PowerPoint
	•	Slide titles
	•	Bullet-point content
	•	Image-based slides
	•	A ready-to-use .pptx file

No manual slide creation needed.

⸻

✨ Features
	•	🤖 Uses Google Gemini (gemini-2.5-pro) for content generation
	•	🖼️ Automatically fetches relevant images from Pexels
	•	📄 Creates structured slides (title, content, image)
	•	⚡ Fully automated PowerPoint generation
	•	🧠 Simple, readable, beginner-friendly Python code

⸻

🛠️ Tech Stack
	•	Python 3.9+
	•	Google Generative AI (Gemini)
	•	python-pptx
	•	Pexels API
	•	requests
	•	python-dotenv

⸻

📁 Project Structure

.
├── main.py              # All-in-one PPT generator script
├── .env                 # API keys (not committed)
├── README.md            # Project documentation


⸻

🔑 Prerequisites

You’ll need API keys for:
	1.	Google Gemini API
	•	Get it from Google AI Studio
	2.	Pexels API
	•	https://www.pexels.com/api/

⸻

🔐 Environment Setup

Create a .env file in the project root:

GEMINI_API_KEY=your_gemini_api_key_here
PEXELS_API_KEY=your_pexels_api_key_here

⚠️ Important:
Never hard-code API keys in your source code.

⸻

📦 Installation

Install required dependencies:

pip install google-generativeai python-pptx python-dotenv requests


⸻

▶️ How to Run

Open main.py and run:

python main.py

By default, it will generate:
	•	Topic: AI in Healthcare
	•	Slides: 6
	•	Output file: ai_healthcare.pptx

You can change this here:

generator.generate_presentation(
    topic="AI in Healthcare",
    num_slides=6,
    output_file="ai_healthcare.pptx"
)


⸻

🧠 How It Works (High Level)
	1.	Gemini AI generates a structured outline in JSON
	2.	Each slide is processed one by one
	3.	Content slides are created using python-pptx
	4.	Image slides fetch relevant images from Pexels
	5.	The final PowerPoint file is saved locally

⸻

📌 Slide Types Supported
	•	title → Title slide
	•	content → Text-based slide
	•	image → Image-focused slide
	•	conclusion → Final summary slide

⸻

🚨 Common Issues

1. Failed to generate outline
	•	Check Gemini API key
	•	You may be rate-limited (free tier)

2. Images not appearing
	•	Check Pexels API key
	•	Some image queries may return no results

3. ModuleNotFoundError
	•	Make sure dependencies are installed correctly

⸻

🚀 Future Improvements
	•	Web interface (FastAPI / Flask)
	•	Custom slide themes
	•	Support for PDFs
	•	Better bullet formatting
	•	One-call AI optimization (reduce API usage)

⸻

🤝 Contributing

Contributions are welcome!
Feel free to:
	•	Open issues
	•	Suggest improvements
	•	Submit pull requests

⸻

📜 License

This project is for educational and personal use.
Make sure you comply with:
	•	Google Gemini API terms
	•	Pexels API usage guidelines

⸻

👤 Author

Divakar Daya
Built with curiosity, caffeine, and AI ☕🤖

⸻

If you want, I can also:
	•	Make this README GSoC / open-source ready
	•	Add screenshots section
	•	Add badges (Python, Gemini, License)
	•	Rewrite it more formally or more startup-style

Just tell me 😄
