# AI Meeting Summarizer

![AI Meeting Summarizer](https://img.shields.io/badge/AI-Meeting%20Summarizer-blue)
![Python](https://img.shields.io/badge/Python-3.8%2B-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 📝 Description

AI Meeting Summarizer is a powerful Streamlit application that leverages the Groq API to automatically extract key insights, action items, and summaries from meeting transcripts or recordings. The tool supports multiple input formats and can provide summaries in 15 different languages.

## ✨ Features

- **Multi-format Support**: Process text files (.txt), documents (.pdf, .docx), audio files (.mp3, .wav, .m4a), and video files (.mp4, .mov, .avi)
- **Automatic Transcription**: Convert audio/video recordings to text using AssemblyAI
- **Intelligent Summarization**: AI-powered extraction of key discussion points
- **Action Item Identification**: Automatically detect tasks, responsible persons, and deadlines
- **Multi-language Support**: Generate summaries in 15 different languages:
  - English, Spanish, French, German, Chinese, Japanese, Russian, Arabic, Hindi, Portuguese, Italian, Dutch, Korean, Swedish, and Turkish
- **PDF Export**: Download professionally formatted summary reports

## 🛠️ Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ai-meeting-summarizer.git
   cd ai-meeting-summarizer
   ```

2. Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up your API keys:
   - Get a Groq API key from [groq.com](https://groq.com)
   - Get an AssemblyAI API key from [assemblyai.com](https://assemblyai.com)

5. Create a `.env` file in the project root and add your API keys:
   ```
   GROQ_API_KEY=your_groq_api_key
   ASSEMBLYAI_API_KEY=your_assemblyai_api_key
   ```

## 📋 Requirements

```
streamlit>=1.25.0
groq>=0.4.0
PyPDF2>=3.0.0
python-docx>=0.8.11
fpdf>=1.7.2
dateparser>=1.1.8
moviepy>=1.0.3
assemblyai>=0.17.0
python-dotenv>=1.0.0
```

## 🚀 Usage

1. Run the Streamlit application:
   ```bash
   streamlit run app.py
   ```

2. Open your web browser and navigate to the local URL displayed in your terminal (typically http://localhost:8501)

3. Upload a meeting transcript or recording file (text, PDF, DOCX, audio, or video)

4. Select your preferred summary language

5. Click "Generate Summary & Action Items" to process the file

6. Review the generated summary and action items

7. Download the PDF report if desired

## 🔄 Workflow

1. **Upload**: User uploads a meeting file (transcript or recording)
2. **Processing**: 
   - For audio/video: The system extracts and transcribes the audio
   - For documents: The system extracts the text content
3. **AI Analysis**: The transcript is processed using the Groq LLM API
4. **Results**: The system displays a summary and structured action items
5. **Export**: User can download a professionally formatted PDF report

## 🧩 How It Works

The application uses several key technologies:
- **Streamlit**: For the interactive web interface
- **Groq API (LLama 3 70B)**: For AI-powered text summarization and analysis
- **AssemblyAI**: For transcribing audio and video files
- **PyPDF2/python-docx**: For extracting text from document files
- **MoviePy**: For extracting audio from video files
- **FPDF**: For generating downloadable PDF reports

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- [Groq](https://groq.com) for their powerful LLM API
- [AssemblyAI](https://assemblyai.com) for their transcription API
- [Streamlit](https://streamlit.io) for the wonderful web app framework

## 📧 Contact

Your Name - Shatadru Dhar - shatadrudhar10c@gmail.com

Project Link: [https://github.com/yourusername/ai-meeting-summarizer](https://github.com/yourusername/ai-meeting-summarizer)
