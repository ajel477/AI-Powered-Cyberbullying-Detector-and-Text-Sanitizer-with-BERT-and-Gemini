# AI-Powered Cyberbullying Detector and Text Sanitizer with BERT and Gemini

A sophisticated machine learning solution that detects and transforms cyberbullying content using BERT (Bidirectional Encoder Representations from Transformers) for classification and Google's Gemini AI for content transformation.

## 🌟 Features

- **Multi-class Cyberbullying Detection**: Identifies different types of cyberbullying:
  - Religion-based
  - Age-based
  - Gender-based
  - Ethnicity-based
  - Other cyberbullying
  - Non-cyberbullying content

- **Platform Support**:
  - YouTube comments and transcripts analysis
  - Twitter tweets analysis
  - Support for text-based content

- **Smart Content Transformation**: Uses Google's Gemini AI to convert negative or harmful content into constructive messages while preserving the core meaning

- **Advanced Text Processing**:
  - Emoji analysis and interpretation
  - Text preprocessing and cleaning
  - Word cloud visualization for different cyberbullying categories

## 🛠️ Technologies Used

- **Machine Learning**: BERT (bert-base-uncased)
- **Deep Learning Framework**: PyTorch
- **Natural Language Processing**: NLTK
- **AI Models**: 
  - BERT for classification
  - Google Gemini 1.5 Flash for content transformation
- **APIs**:
  - YouTube Data API v3
  - Twitter API
  - Google Gemini API

## 📊 Model Performance

- Trained on a comprehensive dataset of labeled tweets
- Implements cross-validation and performance metrics
- Includes confusion matrix visualization
- Supports both batch processing and real-time analysis

## 💻 Installation

1. Clone the repository:
```bash
git clone https://github.com/ajel477/AI-Powered-Cyberbullying-Detector-and-Text-Sanitizer-with-BERT-and-Gemini.git
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Set up API keys in your environment:
```python
DEVELOPER_KEY = "your_youtube_api_key"
GOOGLE_API_KEY = "your_gemini_api_key"
```

## 📈 Usage

### For YouTube Analysis:
```python
from cyberbullying_detector import analyze_youtube_video

youtube_url = 'https://www.youtube.com/watch?v=your_video_id'
results_df = analyze_youtube_video(youtube_url)
```

### For Twitter Analysis:
```python
from cyberbullying_detector import analyze_tweets

results_df = analyze_tweets(tweet_data)
```

## 📋 Features in Detail

1. **Text Preprocessing**:
   - URL removal
   - Special character handling
   - Lowercase conversion
   - Tokenization
   - Stop word removal
   - Lemmatization

2. **Analysis Capabilities**:
   - Emoji interpretation
   - Sentiment analysis
   - Content classification
   - Text transformation

3. **Output Format**:
   - Original text
   - Cyberbullying category
   - Confidence score
   - Transformed content
   - Metadata (author, timestamp, etc.)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- BERT model from Hugging Face Transformers
- Google's Gemini AI for content transformation
- YouTube Data API for video content analysis
- Twitter API for tweet analysis

## ⚠️ Disclaimer

This tool is intended for educational and research purposes. Please use responsibly and in accordance with platform-specific terms of service and API usage guidelines.