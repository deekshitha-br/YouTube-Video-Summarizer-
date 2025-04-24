
**YouTube video summarizerr** is a user-friendly web application developed with Streamlit. It enables users to efficiently summarize the content of YouTube videos by extracting transcript data and generating concise notes using Google Gemini Pro (via the Generative AI API). This tool is particularly useful for students, researchers, and content consumers seeking to save time and gain quick insights from video content.

✨ Key Features

- 🔍 **Transcript Extraction**: Automatically retrieves transcript text from YouTube videos.
- 🧠 **AI-Powered Summarization**: Utilizes Google Gemini Pro to generate structured summaries.
- 📝 **Concise Output**: Delivers bullet-point summaries limited to 250 words for clarity and focus.
- 🖼️ **Visual Cue**: Displays the video thumbnail for easy identification.

⚙️ Getting Started

1. Clone the Repository

```bash
git clone https://github.com/yourusername/youtube-transcript-notes.git
cd youtube-transcript-notes
```

2. Install Dependencies

Install the required Python packages using:

```bash
pip install -r requirements.txt
```

Or manually install them:

```bash
pip install streamlit python-dotenv google-generativeai youtube-transcript-api
```

3. Configure Environment Variables

Create a `.env` file in the project root directory and add your Google API key:

```
GOOGLE_API_KEY=your_google_generative_ai_api_key
```

4. Launch the Application

Start the Streamlit server:

```bash
streamlit run app.py
```

🛠️ Technology Stack

- **Frontend**: [Streamlit](https://streamlit.io/)
- **Backend/AI**: Google Gemini Pro via `google-generativeai`
- **Transcript Extraction**: `youtube-transcript-api`
- **Environment Management**: `python-dotenv`

🧠 Prompt Template for Summarization

```text
You are a YouTube video summarizer. You will be taking the transcript text and summarizing the entire video and providing the important summary in points within 250 words. Please provide the summary of the text given here:
```
📸 Application Preview

Once the application is running:
1. Enter a valid YouTube video URL.
2. Click the "Get Detailed Notes" button.
3. View the video thumbnail and AI-generated notes displayed below.


📌 Notes

- This application currently supports videos that have **English transcripts enabled**.
- Ensure the provided API key has appropriate access to the `gemini-pro` model.
