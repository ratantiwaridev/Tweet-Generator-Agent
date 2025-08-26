# Tweet-Generator-Agent
An interactive Tweet Generator Agent powered by Google Gemini API and ipywidgets.
It allows you to create customized tweets with different tones, audiences, and hashtags — all under 280 characters!

🚀 Features

Generate tweets on any topic with AI ✨

Choose tone: Professional, Casual, Motivational, Witty, Informative

Define target audience 🎯

Add hashtags for reach 📢

Interactive form using ipywidgets inside Jupyter/Colab

Outputs are styled with Markdown for readability

📦 Installation

Run the following inside Colab or Jupyter Notebook:

!pip install google-generativeai --quiet
!pip install ipywidgets --quiet

⚙️ Setup

Get your API key from Google AI Studio
.

Replace the placeholder in the notebook:

API_KEY = "your_api_key_here"
genai.configure(api_key=API_KEY)


The model used is:

model = genai.GenerativeModel("gemini-2.5-flash")

📝 Usage

Run the notebook cells step by step:

Install dependencies

Import required libraries

Configure Gemini API key

Fill in the form fields:

Topic (e.g., "AI in Healthcare")

Tone (choose from dropdown)

Audience (e.g., "Tech Enthusiasts")

Hashtags (comma-separated)

Click Generate Tweet

Example prompt inside code:

prompt=f"""
You are an expert content writer. Generate a tweet about this topic "{topic_input.value}".
Use a tone {Descr_input.value}.
Generate tweet for audience {audience_input.value}.
Include the hashtags {hashtag_input.value}.
Keep it humorous and under 280 characters.
"""

📸 Demo

When you run the notebook, you’ll see a form like this:

Tweet Generator Agent
[ Topic  ]  
[ Tone (dropdown) ]  
[ Audience ]  
[ Hashtag ]  
[ Generate Tweet Button ]  


After clicking Generate Tweet, the AI will return a ready-to-use tweet 🎉

📌 Example Output

Generated Tweet:
"AI in healthcare is like having a doctor who never sleeps 🩺🤖. Smarter diagnoses, faster decisions, better care. Future is now! #AI #Healthcare #Innovation"

📂 Project Structure
Tweet-Generator-Agent/
│── Ratan's_Simple_agent.ipynb   # Main Colab notebook
│── README.md                    # Project documentation

🛠️ Tech Stack

Google Gemini API

ipywidgets

Python 3.x

Jupyter/Colab

🙌 Acknowledgments

Google Generative AI for the Gemini model

Jupyter + Colab for making interactive notebooks simple

Inspiration from the idea of AI-powered content creation

⚡ Pro Tip: Fork this repo and customize prompts to generate blog ideas, LinkedIn posts, or ad copy — not just tweets!
