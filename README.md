# Data Analyst - AI-Powered FastAPI Application

A comprehensive data analysis application built with FastAPI that integrates Gemini AI and OCR capabilities for intelligent data processing and analysis.

## Features

- 🤖 **AI-Powered Analysis**: Uses Google Gemini AI for intelligent data interpretation
- 📄 **OCR Integration**: Extract text from images and documents using OCR.space API
- 📊 **Data Processing**: Handles various data formats (CSV, JSON, Excel, etc.)
- 🚀 **FastAPI Backend**: High-performance async web framework
- 🔄 **File Upload**: Support for multiple file formats and data sources
- 📈 **Data Visualization**: Generate charts and graphs from your data

## Setup

### Prerequisites

- Python 3.8+
- pip package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/22f3000982/tds_proj2.git
cd tds_proj2
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
Create a `.env` file in the root directory with your API keys:
```
gemini_api=your_gemini_api_key_here
OCR_API_KEY=your_ocr_api_key_here
API_KEY=your_additional_api_key_here
```

4. Run the application:
```bash
python app.py
```

The application will start on `http://localhost:8000`

## API Documentation

Once the server is running, visit `http://localhost:8000/docs` to access the interactive API documentation (Swagger UI).

## Project Structure

```
├── app.py                 # Main FastAPI application
├── data_scrape.py         # Data scraping utilities
├── requirements.txt       # Python dependencies
├── .env                  # Environment variables (not in repo)
├── .gitignore           # Git ignore rules
├── LICENSE              # License file
└── prompts/             # AI prompt templates
    ├── task_breaker.txt
    └── unified_code_instructions.txt
```

## Usage

### Basic Data Analysis
Send a POST request to `/aianalyst/` with your data files and questions to get AI-powered insights.

### OCR Processing
Upload images or documents to extract text using the integrated OCR functionality.

## Technologies Used

- **FastAPI**: Modern, fast web framework for building APIs
- **Google Gemini AI**: Advanced language model for data analysis
- **OCR.space API**: Optical Character Recognition service
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Matplotlib/Seaborn**: Data visualization
- **DuckDB**: In-process SQL OLAP database management system

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## API Keys Setup

To use this application, you'll need to obtain API keys from:

1. **Google Gemini AI**: Visit [Google AI Studio](https://ai.google.dev/) to get your API key
2. **OCR.space**: Sign up at [OCR.space](https://ocr.space/ocrapi) for your OCR API key

Add these keys to your `.env` file as shown in the setup instructions.
