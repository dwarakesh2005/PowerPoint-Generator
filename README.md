# PowerPoint Generator - Text to Presentation

## 🚀 Transform Your Text into Stunning Presentations with AI

A powerful web application that converts bulk text, markdown, or prose into fully formatted PowerPoint presentations using AI-powered content analysis and template styling.

### ✨ Live Demo
[Try the app here](https://your-username.github.io/powerpoint-generator)

## 🎯 Features

### Core Functionality
- **Smart Text Analysis**: Intelligently breaks down input text into logical slide structure
- **AI-Powered Content Generation**: Uses advanced AI to create engaging slide content
- **Template Style Extraction**: Automatically applies colors, fonts, and layouts from uploaded templates
- **Multiple Output Formats**: Generates downloadable .pptx files
- **Real-time Preview**: See your slides before downloading

### 🎁 Bonus Features (For Extra Credit)
- **🎤 Auto-Generated Speaker Notes**: AI creates detailed talking points for each slide
- **🎨 Multiple Style Templates**: Pre-built templates for different use cases:
  - 💼 Investor Pitch Decks
  - 🔬 Technical Reports  
  - 💰 Sales Presentations
  - 📚 Educational Content
  - 📈 Marketing Decks
  - 🔍 Research Summaries
- **👀 Live Slide Previews**: Visual preview of all slides before download
- **⚙️ Advanced Options**: 
  - Custom slide count
  - Speaker notes toggle
  - Slide transitions
  - Image optimization
- **🛡️ Robust Error Handling**: Comprehensive validation and fallback mechanisms
- **📱 Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **🔒 Privacy-First**: No data storage, secure API handling

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **File Processing**: JSZip for PowerPoint file generation
- **AI Integration**: OpenAI GPT-4 (with fallback support for Claude, Gemini)
- **Template Analysis**: Custom XML parsing for PPTX style extraction
- **File Downloads**: FileSaver.js for client-side file generation

## 📖 How It Works

### 1. Text Parsing and Analysis
The application uses a multi-step approach to convert text into presentation structure:

1. **Content Segmentation**: Analyzes input text for natural breakpoints (headers, paragraphs, topics)
2. **Semantic Understanding**: AI identifies key concepts, relationships, and logical flow
3. **Slide Mapping**: Intelligently determines optimal number of slides based on content density
4. **Content Optimization**: Converts long-form text into bullet-friendly, presentation-ready format

### 2. Template Style Application
The app extracts and applies visual styles from uploaded PowerPoint templates:

1. **XML Parsing**: Decompresses PPTX files and parses theme.xml for color schemes
2. **Font Extraction**: Identifies title and body fonts from slide masters
3. **Layout Analysis**: Examines slide layouts and placeholder positioning
4. **Asset Management**: Catalogs and reuses images, shapes, and design elements
5. **Style Inheritance**: Applies extracted styles to newly generated content while maintaining template aesthetics

### 3. PowerPoint Generation Process
1. **Structure Creation**: Builds complete PPTX file structure with proper relationships
2. **Content Integration**: Populates slides with AI-generated content
3. **Style Application**: Applies template-extracted themes and formatting
4. **File Assembly**: Creates downloadable PPTX using industry-standard XML schemas

## 🚀 Quick Start

### Online Usage (Recommended)
1. Visit the [live demo](https://your-username.github.io/powerpoint-generator)
2. Paste your content in the text area
3. Choose a style template or add custom guidance
4. Optionally upload a PowerPoint template for custom styling
5. Click "Generate PowerPoint Presentation"
6. Preview and download your presentation

### Local Development
```bash
git clone https://github.com/your-username/powerpoint-generator.git
cd powerpoint-generator
python -m http.server 8000  # or use any local server
open http://localhost:8000
```

## 🔧 Configuration

### Default AI Setup
The app comes pre-configured with OpenAI access - no setup required for basic usage.

### Custom AI Providers
Support for multiple AI providers:
- **OpenAI**: GPT-4, GPT-3.5-turbo
- **Anthropic**: Claude models
- **Google**: Gemini Pro

Simply select your provider and enter your API key.

## 📁 Project Structure

```
powerpoint-generator/
├── index.html              # Main application
├── README.md               # This documentation
├── LICENSE                 # MIT License
├── docs/                   # Additional documentation
│   ├── technical-guide.md  # Technical implementation details
│   └── api-integration.md  # API integration guide
└── examples/               # Sample templates and outputs
    ├── templates/          # Sample PowerPoint templates
    └── outputs/            # Example generated presentations
```

## 🎨 Supported Template Styles

The application intelligently adapts to various PowerPoint template styles:

- **Corporate Templates**: Professional business presentations
- **Creative Templates**: Colorful, modern designs with custom graphics
- **Academic Templates**: Clean, scholarly presentation formats
- **Marketing Templates**: Brand-focused layouts with visual emphasis
- **Technical Templates**: Data-heavy, chart-friendly designs

## 🔒 Privacy & Security

- **No Data Storage**: Content and API keys are never stored or logged
- **Client-Side Processing**: All operations happen in your browser
- **Secure API Handling**: API keys are used only for the current session
- **No Tracking**: No analytics or user tracking implemented

## 🐛 Troubleshooting

### Common Issues

**"API request failed"**
- Verify your API key is correct and has sufficient credits
- Check your internet connection
- Try switching to demo mode for testing

**"Template analysis failed"**
- Ensure uploaded file is a valid .pptx or .potx file
- Try with a smaller template file (< 50MB)
- The app will use default styling if template analysis fails

**"Invalid content format"**
- Ensure you have at least 50 characters of content
- Try breaking up very long text into paragraphs
- Check for special characters that might cause parsing issues

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Development Setup
1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and test thoroughly
4. Submit a pull request with a clear description

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- OpenAI for GPT-4 API
- JSZip library for PowerPoint file generation
- FileSaver.js for client-side downloads
- The open-source community for inspiration and tools

## 📧 Support

For support, feature requests, or bug reports:
- Open an issue on GitHub
- Check our [FAQ](docs/faq.md)
- Review the [Technical Guide](docs/technical-guide.md)

---

**Built with ❤️ for seamless presentation creation**
