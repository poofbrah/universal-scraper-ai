# universal-scraper-ai
Universal Web Scraper Integrated with LLMs
A powerful, customizable web scraper built with Selenium and Streamlit, leveraging Large Language Models (LLMs) to extract and structure data. The project provides a simple interface to scrape websites, process the content, and download the results in various formats.

Features
Scraping: Uses Selenium to navigate websites and fetch HTML content.
LLM Integration: Formats extracted data using language models for intelligent data structuring.
Streamlit Interface: User-friendly interface for setting up and running the scraper.
Export Options: Save results as JSON, CSV, or Markdown files.
Requirements
Install the required packages using the provided requirements.txt file:

bash
pip install -r requirements.txt

Installation
Step 1: Clone the repository
bash git clone https://github.com/poofbrah/universal-web-scraper.git
     cd universal-web-scraper
Step 2: Set up the environment
     Create a .env file in the root directory with the following keys (replace with your actual keys):
OPENAI_API_KEY=your_openai_api_key
GOOGLE_API_KEY=your_google_api_key
GROQ_API_KEY=your_groq_api_key
Ensure that the ChromeDriver(can be downloaded from the chrome website) path in scraper.py is correctly set to your local ChromeDriver executable.

Step 3: Run the Streamlit application
To launch the web interface, run:

bash/terminal
streamlit run streamlit_app.py
This will open the Streamlit application in your browser.

Usage
Open the Streamlit Interface: Enter the URL you want to scrape, choose a model, and specify the fields to extract.
Start Scraping: Click the Scrape button on the sidebar to begin scraping. The application will display the extracted data, as well as the token usage and estimated cost based on the model selected.
Download Results: After scraping, download the results in your preferred format (JSON, CSV, or Markdown).

Project Structure
assets.py: Contains configuration variables and constants used across the project.
scraper.py: Handles the web scraping logic and data processing.
streamlit_app.py: Provides the Streamlit interface for user interaction.
.env: (not included in the repository) Stores API keys for OpenAI, Google, and Groq integrations.
requirements.txt: Lists all the dependencies needed to run the project.
Additional Notes
User Agents: assets.py contains a list of user agents to simulate different browsers and devices during scraping​(assets).
Model Pricing: Model-specific pricing details are included in assets.py, which estimates costs based on token usage​(assets).
WebDriver Path: Ensure the ChromeDriver path in scraper.py matches your local setup for Selenium to function properly​(scraper).
License
This project is licensed under the MIT License.

Contact
For questions or further information, please reach out at [psp5205@psu.edu].
