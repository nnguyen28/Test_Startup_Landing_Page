# Test_Startup_Landing_Page
This project is designed to transform traditional CRM systems into AI-driven decision engines.

Instead of just storing customer data, this system:

Understands customer behavior
Predicts future actions
Automates engagement at scale

💡 Built for startups, SMBs, and enterprise teams looking to modernize their customer relationship strategy.

# Import necessary libraries
import os
import warnings
from IPython.display import display, Markdown, HTML  # For displaying HTML directly
from dotenv import load_dotenv

# Import specific clients/modules for each provider
from openai import OpenAI
import google.generativeai as genai
from anthropic import Anthropic

# Load environment variables from the .env file
load_dotenv()
print("Attempting to load API keys from .env file...")

# Load Keys
openai_api_key = os.getenv("OPENAI_API_KEY")

# OpenAI Client (Refresher)
openai_client = OpenAI(api_key = openai_api_key)
print(f"OpenAI Client configured (Key starts with: {openai_api_key[:5]}...).")
