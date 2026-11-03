# 🎥 YouTube Video Analyzer Agent

An AI-powered YouTube video analysis application built using **Python, Agno, Groq, and Qwen**. It analyzes YouTube videos by retrieving video metadata and captions, then generates structured summaries, topic-wise explanations, and chapter breakdowns.

The application uses an AI agent to transform lengthy YouTube videos into organized and easy-to-understand information.

## 🚀 Live Demo

**Try the application:** [YouTube Video Analyzer – Streamlit App](ADD_YOUR_STREAMLIT_URL_HERE)

## ✨ Features

- **Video Metadata Extraction:** Retrieves video information such as title, channel, and duration.
- **Caption Retrieval:** Fetches available YouTube captions and transcripts.
- **AI-Powered Video Analysis:** Uses an LLM to understand and explain video content.
- **Chapter Breakdown:** Organizes video content into meaningful topic-based sections.
- **Timestamp Analysis:** Uses available timestamp information to identify important sections of a video.
- **Key Takeaways:** Extracts important concepts, explanations, and learning points.
- **Structured Output:** Presents the analysis using Markdown headings, lists, and tables.

## 🧠 How It Works

The application follows an agent-based workflow:

1. **User Input:** The user provides a YouTube video URL.
2. **Agent Initialization:** Agno initializes the YouTube Analyzer Agent.
3. **Metadata Extraction:** YouTube tools retrieve the video's metadata.
4. **Caption Retrieval:** The agent retrieves available captions.
5. **LLM Processing:** Groq-powered Qwen analyzes the retrieved information.
6. **Content Organization:** The model generates summaries, identifies major topics, and organizes the content into chapters.
7. **Final Output:** The results are displayed through the Streamlit interface.

## 🏗️ Architecture

```text
          User
           |
           v
    Streamlit Interface
           |
           v
    YouTube Analyzer Agent
           |
           v
       Agno Framework
           |
       +---+---+
       |       |
       v       v
  YouTube    Groq API
   Tools        |
       |        v
       |      Qwen LLM
       |        |
       +----+---+
            |
            v
     Video Analysis
            |
            v
     Structured Output
            |
            v
     Streamlit UI
```

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Agno | AI agent framework |
| Groq API | LLM inference |
| Qwen | Language model |
| YouTube Tools | Video metadata and caption retrieval |
| Streamlit | Web application interface |
| python-dotenv | Environment variable management |

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/Krish07chawla/Youtube_Video_Analyzer_Agent.git
```

### 2. Navigate to the project

```bash
cd Youtube_Video_Analyzer_Agent
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Configure API keys

Create a `.env` file in the root directory:

```env
GROQ_API_KEY=your_groq_api_key
```

Never upload your `.env` file or expose your API keys publicly.

### 6. Run the application

```bash
streamlit run ui.py
```

Open the local URL displayed in your terminal to use the application.

## ⚠️ Limitations

- Transcript retrieval depends on the availability and accessibility of YouTube captions.
- Some videos may not provide accessible transcripts.
- YouTube may temporarily restrict or fail transcript requests.
- Accurate chapter timestamps depend on the availability of actual caption timing information.
- AI-generated explanations should be checked against the original video for critical information.

## 🔮 Future Improvements

- Improve timestamp accuracy and chapter segmentation.
- Support multiple languages and translated transcripts.
- Implement Retrieval-Augmented Generation (RAG).
- Add downloadable video summaries and transcripts.
- Support longer videos and improved transcript processing.
- Introduce conversational question answering over video content.

## 🎯 Learning Outcomes

This project explores practical implementation of:

- Agentic AI and autonomous workflows.
- LLM integration using Groq.
- Tool calling and external API integration.
- Prompt engineering and structured outputs.
- Video transcript processing.
- AI-powered application development.
- Deployment using Streamlit Community Cloud.

## 👨‍💻 Author

**Krish Chawla**
 Exploring Agentic AI, Generative AI, Machine Learning, and LLM Applications.

GitHub: [@Krish07chawla](https://github.com/Krish07chawla)

---

⭐ If you find this project useful, feel free to explore the repository and try the live application!
