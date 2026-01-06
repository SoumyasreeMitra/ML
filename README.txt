
AI-Powered PowerPoint Generator using Gemini & Pexels

This project is a Python-based automated PowerPoint generator that creates professional presentation slides using Google Gemini AI for content generation and the Pexels API for fetching relevant images.

By providing a single topic, the system automatically generates:
- Slide titles
- Bullet-point content
- Structured slide layouts
- Relevant stock images
- A downloadable .pptx file

--------------------------------------------------

FEATURES
- AI-generated slide content using Google Gemini
- Automatic PowerPoint creation using python-pptx
- Free stock images fetched via Pexels API
- Secure API key handling using environment variables
- Graceful fallback mechanism when AI or image APIs fail
- Fully automated end-to-end PPT generation

--------------------------------------------------

TECHNOLOGIES USED
- Python 3
- Google Gemini API (google-generativeai)
- Pexels REST API
- python-pptx
- Requests
- Pillow (PIL)
- dotenv / Environment Variables

--------------------------------------------------

PROJECT STRUCTURE
- main.ipynb / main.py : Main script or notebook
- README.txt          : Project documentation
- .env                : API keys (not uploaded to GitHub)
- output.pptx         : Generated presentation

--------------------------------------------------

API KEYS REQUIRED

1. Google Gemini API Key
   - Used for generating slide content
   - Get from: https://aistudio.google.com
   - Environment variable: GEMINI_API_KEY

2. Pexels API Key
   - Used for downloading images
   - Get from: https://www.pexels.com/api/
   - Environment variable: PEXELS_API_KEY

IMPORTANT: Do not hardcode API keys in source code.

--------------------------------------------------

SETUP INSTRUCTIONS

1. Install dependencies:
   pip install google-generativeai python-pptx Pillow requests python-dotenv

2. Set API keys:
   import os
   os.environ["GEMINI_API_KEY"] = "YOUR_GEMINI_API_KEY"
   os.environ["PEXELS_API_KEY"] = "YOUR_PEXELS_API_KEY"

3. Run the project:
   topic = "Artificial Intelligence in Healthcare"
   num_slides = 6
   generator.generate_presentation(topic, num_slides, "AI_Healthcare_Presentation.pptx")

--------------------------------------------------

OUTPUT
- A fully formatted PowerPoint (.pptx) file
- Includes title, content, conclusion slides and images

--------------------------------------------------

ERROR HANDLING
- Gemini API rate limits handled using fallback outline
- Image download failures handled using placeholders
- Program does not crash on API errors

--------------------------------------------------

USE CASES
- College mini / major projects
- Seminar and presentation automation
- AI workflow demonstrations
- Learning API integration

--------------------------------------------------

LICENSE
This project is for educational purposes.
Pexels images are free to use under the Pexels license.

--------------------------------------------------

ACKNOWLEDGEMENTS
- Google Gemini AI
- Pexels Free Stock Images
- python-pptx Library
