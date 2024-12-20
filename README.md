# YouTube Video Summarizer 🎥 ✍️

A Streamlit web application that converts YouTube video transcripts into concise, detailed notes using Google's Gemini AI. This tool helps users quickly grasp the key points of any YouTube video without watching the entire content.

## 🌟 Features

- Clean and intuitive web interface powered by Streamlit
- Automatic YouTube transcript extraction
- AI-powered summarization using Google's Gemini-1.5-Flash model
- Video thumbnail preview
- Concise summaries within 250 words
- Real-time processing

## 🚀 Getting Started

### Prerequisites

Install the required Python packages:

```bash
pip install streamlit
pip install google-generativeai
pip install python-dotenv
pip install youtube-transcript-api
```

### Environment Setup

1. Create a `.env` file in the root directory
2. Add your Google API key:
```
GOOGLE_API_KEY=your_api_key_here
```

### Running the Application

1. Clone the repository
2. Navigate to the project directory
3. Run the Streamlit app:
```bash
streamlit run app.py
```

## 💡 How to Use

1. Launch the application
2. Enter a YouTube video URL in the input field
3. Click "Get Detailed Notes" button
4. View the AI-generated summary of the video content

## ⚙️ Technical Components

### Key Dependencies

- `streamlit`: Web application framework
- `google.generativeai`: Google's Gemini AI API
- `youtube_transcript_api`: YouTube transcript extraction
- `python-dotenv`: Environment variable management

### Core Functions

1. **extract_transcript_details()**
   - Extracts video ID from URL
   - Retrieves transcript using YouTube API
   - Concatenates transcript text

2. **generate_gemini_content()**
   - Initializes Gemini AI model
   - Processes transcript text
   - Returns summarized content

## 🔑 API Keys

To use this application, you'll need:
1. Google API key for Gemini AI
   - Get it from [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Add it to your `.env` file

## 🛠️ Error Handling

The application includes error handling for:
- Invalid YouTube URLs
- Missing transcripts
- API failures
- Invalid API keys

## 📝 Notes

- Summaries are limited to 250 words
- Only works with YouTube videos that have available transcripts
- Requires stable internet connection for API calls

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open-source and available under the MIT License.

## ⚠️ Limitations

- Only works with public YouTube videos
- Requires videos to have transcripts available
- API rate limits may apply
- English language transcripts preferred for best results

## 🙏 Acknowledgments

- Google Gemini AI team
- Streamlit developers
- YouTube Transcript API developers

## 📞 Support

For issues and feature requests, please open an issue in the repository.