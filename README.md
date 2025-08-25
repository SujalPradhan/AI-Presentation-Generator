# Auto PPT Generator - Complete Project Structure

## File Structure
```
auto-ppt-generator/
├── index.html              # Main application file
├── README.md              # Setup and usage instructions
├── LICENSE                # MIT License
├── package.json           # Project configuration
├── assets/
│   ├── demo-template.pptx # Sample template for testing
│   └── screenshots/       # App screenshots for README
├── docs/
│   └── writeup.md        # Technical write-up
└── .github/
    └── workflows/
        └── deploy.yml     # GitHub Pages deployment
```

---

## README.md

# 🎯 Auto PPT Generator

Transform your text into professional PowerPoint presentations instantly using AI and custom templates.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Try%20Now-blue)](https://your-username.github.io/auto-ppt-generator)
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GitHub Stars](https://img.shields.io/github/stars/your-username/auto-ppt-generator)](https://github.com/your-username/auto-ppt-generator/stargazers)

## ✨ Features

- **AI-Powered Content Analysis**: Intelligently converts bulk text, markdown, or prose into structured slides
- **Free Tier Support**: Works with free API tiers from OpenAI, Anthropic, and Google
- **Cost-Effective**: Uses optimized models (GPT-3.5-Turbo, Claude 3 Haiku, Gemini 1.5 Flash)
- **Template Integration**: Preserves your PowerPoint template's styles, colors, fonts, and layouts
- **Secure Processing**: API keys processed in-browser only - never stored or logged
- **Live Preview**: See slide structure before generating final presentation
- **Speaker Notes**: Auto-generates speaker notes for enhanced presentations

## 🚀 Quick Start

### Option 1: Use the Hosted Demo
Visit the [live demo](https://your-username.github.io/auto-ppt-generator) and start generating presentations immediately.

### Option 2: Run Locally
```bash
# Clone the repository
git clone https://github.com/your-username/auto-ppt-generator.git
cd auto-ppt-generator

# Serve locally (choose one method)
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000

# Open http://localhost:8000 in your browser
```

## 📋 Usage Instructions

### Step 1: Prepare Your Content
- Paste or type your text content (supports markdown and prose)
- Content can be structured (with headers) or unstructured
- Typical length: 500-5000 words for optimal slide generation

### Step 2: Configure AI Settings
- Select your preferred AI provider (OpenAI, Anthropic, or Gemini)
- Enter your API key (processed securely in-browser only)
- Choose a tone preset or provide custom guidance

### Step 3: Upload Template
- Upload a PowerPoint template (.pptx or .potx file)
- Template should contain the desired styles, colors, and layouts
- Maximum file size: 50MB

### Step 4: Generate Presentation
- Click "Generate PowerPoint Presentation"
- Review the slide preview
- Download your customized .pptx file

## 🔑 API Key Requirements

You'll need an API key from one of these providers (all offer free tiers):

- **OpenAI (Recommended)**: [Get API Key](https://platform.openai.com/api-keys) 
  - **Free Tier**: $5 in free credits for new accounts
  - **Model**: GPT-3.5-Turbo (faster and more cost-effective than GPT-4)
  - **Cost**: ~$0.002 per presentation

- **Anthropic**: [Get API Key](https://console.anthropic.com/) 
  - **Free Tier**: Available with rate limits
  - **Model**: Claude 3 Haiku (fastest and most affordable Claude model)
  - **Cost**: Very low cost per presentation

- **Google Gemini**: [Get API Key](https://makersuite.google.com/app/apikey) 
  - **Free Tier**: 15 requests per minute, 1500 per day
  - **Model**: Gemini 1.5 Flash (optimized for speed and efficiency)
  - **Cost**: Free within limits

**Security Note**: API keys are processed entirely in your browser and are never transmitted to our servers or stored anywhere.

## 🛠️ Technical Details

### Architecture
- **Frontend**: Pure HTML5, CSS3, and JavaScript (ES6+)
- **PowerPoint Generation**: JSZip library for PPTX file manipulation
- **AI Integration**: Direct API calls to LLM providers
- **Processing**: Client-side only - no backend required

### Key Libraries
- [JSZip](https://stuk.github.io/jszip/) - PowerPoint file generation
- Native Fetch API - LLM communication
- CSS Grid & Flexbox - Responsive layout

### Browser Compatibility
- Chrome 70+ ✅
- Firefox 65+ ✅
- Safari 12+ ✅
- Edge 79+ ✅

## 📁 Sample Content for Testing

```markdown
# Company Overview
Our startup revolutionizes digital marketing through AI-powered analytics.

## Problem Statement
- Traditional marketing lacks real-time insights
- Manual analysis is time-consuming and error-prone
- ROI tracking across channels is fragmented

## Our Solution
We provide an integrated platform that:
- Analyzes customer behavior in real-time
- Predicts optimal marketing spend allocation
- Delivers actionable insights through AI

## Market Opportunity
The global marketing analytics market is worth $3.2B and growing at 12% annually.

## Financial Projections
Year 1: $500K ARR
Year 2: $2M ARR  
Year 3: $8M ARR
```

## 🎨 Customization

### Adding New Tone Presets
Edit the `toneMap` object in the JavaScript to add custom tone options:

```javascript
const toneMap = {
    'your-tone': 'Your custom guidance for the AI'
};
```

### Modifying Slide Generation
The slide generation logic is in the `processTextWithLLM()` method. Customize the prompt to change how content is structured.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Development Setup
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [JSZip](https://stuk.github.io/jszip/) for PowerPoint file manipulation
- [OpenXML SDK](https://docs.microsoft.com/en-us/office/open-xml/open-xml-sdk) documentation
- AI providers for their excellent APIs

## 📞 Support

- Create an [issue](https://github.com/your-username/auto-ppt-generator/issues) for bug reports
- Star ⭐ this repository if you find it helpful
- Share with others who might benefit from automated presentation generation

---

**Made with ❤️ for the open source community**

---

## LICENSE (MIT)

```
MIT License

Copyright (c) 2025 Auto PPT Generator

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## package.json

```json
{
  "name": "auto-ppt-generator",
  "version": "1.0.0",
  "description": "Transform your text into professional PowerPoint presentations instantly using AI and custom templates",
  "main": "index.html",
  "scripts": {
    "start": "python -m http.server 8000",
    "serve": "npx serve .",
    "deploy": "gh-pages -d ."
  },
  "repository": {
    "type": "git",
    "url": "https://github.com/your-username/auto-ppt-generator.git"
  },
  "keywords": [
    "powerpoint",
    "presentation",
    "ai",
    "automation",
    "pptx",
    "openai",
    "claude",
    "gemini",
    "slides"
  ],
  "author": "Your Name",
  "license": "MIT",
  "bugs": {
    "url": "https://github.com/your-username/auto-ppt-generator/issues"
  },
  "homepage": "https://your-username.github.io/auto-ppt-generator",
  "devDependencies": {
    "gh-pages": "^6.0.0"
  }
}
```

---

## .github/workflows/deploy.yml (GitHub Pages Deployment)

```yaml
name: Deploy to GitHub Pages

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  deploy:
    runs-on: ubuntu-latest
    
    steps:
    - uses: actions/checkout@v3
    
    - name: Setup Node.js
      uses: actions/setup-node@v3
      with:
        node-version: '18'
        
    - name: Deploy to GitHub Pages
      uses: peaceiris/actions-gh-pages@v3
      if: github.ref == 'refs/heads/main'
      with:
        github_token: ${{ secrets.GITHUB_TOKEN }}
        publish_dir: ./
        exclude_assets: '.github,node_modules,*.md'
```