# GenAI Medical Imaging Agent 🏥📸

A powerful AI-driven medical image analysis tool built with Streamlit and Google's Gemini AI model. This application provides detailed analysis of medical images including X-rays, MRIs, CT scans, and ultrasounds with comprehensive diagnostic insights.

## Features ✨

- **Multi-Modal Image Analysis**: Supports various medical imaging formats (X-ray, MRI, CT, Ultrasound, etc.)
- **Comprehensive Reporting**: Structured analysis including:
  - Image type and region identification
  - Key findings and abnormalities
  - Diagnostic assessment with confidence levels
  - Patient-friendly explanations
  - Research context with recent medical literature
- **Interactive Web Interface**: User-friendly Streamlit interface for easy image upload and analysis
- **AI-Powered Insights**: Leverages Google's Gemini 2.0 Flash model for accurate medical interpretations
- **Research Integration**: Automatic search for relevant medical literature using DuckDuckGo

## Prerequisites 📋

- Python 3.8+
- Google API Key for Gemini model
- Internet connection (for research capabilities)

## Installation 🚀

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd "GenAI medical imaging agent"
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install required dependencies**
   ```bash
   pip install streamlit pillow agno python-dotenv
   ```

4. **Set up environment variables**
   Create a `.env` file in the project root and add your Google API key:
   ```
   GOOGLE_API_KEY=your_google_api_key_here
   ```

## Usage 💻

1. **Start the application**
   ```bash
   streamlit run main.py
   ```

2. **Access the web interface**
   - Open your browser and navigate to `http://localhost:8501`

3. **Upload and analyze**
   - Use the sidebar to upload a medical image (JPG, PNG, BMP, GIF formats supported)
   - Click "Analyze Image" to get comprehensive analysis
   - Review the detailed report with findings and recommendations

## How It Works 🔍

1. **Image Processing**: The application resizes uploaded images for optimal AI processing
2. **AI Analysis**: Uses Google's Gemini 2.0 Flash model to analyze medical images
3. **Structured Reporting**: Generates comprehensive reports with:
   - Technical image assessment
   - Medical findings and abnormalities
   - Diagnostic recommendations
   - Patient-friendly explanations
   - Supporting research literature
4. **Research Integration**: Automatically searches for relevant medical studies and treatment protocols

## Supported Image Types 📁

- **Formats**: JPG, JPEG, PNG, BMP, GIF
- **Modalities**: X-rays, MRI, CT scans, Ultrasounds, and other medical imaging types
- **Anatomical Regions**: All body systems and regions

## Important Disclaimers ⚠️

- **Not for Clinical Diagnosis**: This tool is for educational and research purposes only
- **Medical Professional Required**: Always consult qualified healthcare professionals for medical decisions
- **AI Limitations**: AI analysis should supplement, not replace, professional medical judgment
- **Privacy**: Ensure compliance with healthcare data regulations (HIPAA, GDPR, etc.)

## Project Structure 📂

```
GenAI medical imaging agent/
├── main.py              # Main Streamlit application
├── .env                 # Environment variables (create this)
├── .gitignore          # Git ignore rules
├── README.md           # This file
└── requirements.txt    # Python dependencies (optional)
```

## Dependencies 📦

- **streamlit**: Web interface framework
- **pillow**: Image processing library
- **agno**: AI agent framework
- **python-dotenv**: Environment variable management
- **google-generativeai**: Google Gemini AI model (via agno)

## Contributing 🤝

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License 📄

This project is licensed under the MIT License - see the LICENSE file for details.

## Support 🆘

If you encounter any issues or have questions:
- Check the GitHub Issues page
- Ensure your Google API key is properly configured
- Verify all dependencies are correctly installed

## Acknowledgments 🙏

- Google for the Gemini AI model
- Streamlit for the excellent web framework
- The medical imaging community for inspiring this tool

---

**Remember**: This tool is for educational purposes. Always consult healthcare professionals for medical decisions. 