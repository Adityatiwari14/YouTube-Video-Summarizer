# YouTube Video Summarizer

## Overview
This project extracts transcripts from YouTube videos and generates a concise summary using Google Gemini Pro. It is built using Streamlit for an interactive web-based user experience.

## Project Structure
- `.env` - Contains API keys and environment variables.
- `app.py` - The main Streamlit web application for processing YouTube video transcripts.
- `requirements.txt` - Dependencies required to run the project.

## Features
- Extracts video transcripts using `youtube_transcript_api`.
- Generates a summarized version of the transcript using Google Gemini Pro.
- Provides a user-friendly web interface with Streamlit.
- Displays the video thumbnail for easy identification.

## Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up environment variables:
   - Create a `.env` file in the project root.
   - Add the Google API key:
     ```
     GOOGLE_API_KEY="your_google_api_key_here"
     ```

## Usage
1. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```
2. Enter the YouTube video link in the text input box.
3. Click the "Get Detailed Notes" button to extract and summarize the transcript.
4. View the summary in bullet points within 250 words.

## Explanation of Files
### `.env`
- Stores the `GOOGLE_API_KEY` used for accessing the Google Gemini Pro API.
- **Ensure this file is not shared publicly to protect sensitive credentials.**

### `app.py`
- Loads environment variables using `dotenv`.
- Extracts YouTube video transcripts using `youtube_transcript_api`.
- Generates a summarized version of the transcript using Google Gemini Pro.
- Displays the YouTube thumbnail and summary in a user-friendly interface.

### `requirements.txt`
- Lists all required dependencies:
  - `youtube_transcript_api`: Extracts YouTube video transcripts.
  - `streamlit`: Creates an interactive web app.
  - `google-generativeai`: Connects to Google Gemini Pro for generating summaries.
  - `python-dotenv`: Manages environment variables.
  - `pathlib`: Handles file path operations.

## Contributing
Contributions are welcome! Feel free to submit issues and pull requests to improve the project.

## License
This project is licensed under the MIT License. See `LICENSE` for details.
