# 🚀 AI Business Analyzer

An intelligent business analysis tool powered by Google's Gemini AI that helps entrepreneurs and business professionals generate ideas, analyze markets, and make data-driven decisions.

![AI Business Analyzer](https://img.shields.io/badge/AI-Business%20Analyzer-blue)
![Python](https://img.shields.io/badge/Python-3.9+-green)
![Flask](https://img.shields.io/badge/Flask-3.0.0-lightgrey)
![Gemini](https://img.shields.io/badge/Google-Gemini%202.5%20Pro-orange)

## ✨ Features

- **💡 AI-Powered Business Insights**: Generate unique business ideas and comprehensive market analysis
- **📊 Data Analysis**: Upload and analyze business data files (CSV, TXT, JSON)
- **📈 Visual Analytics**: Automatic chart generation for financial data visualization
- **💬 Conversational Interface**: Natural language interaction with context-aware responses
- **📝 Chat History**: Save and resume previous conversations
- **🎨 Modern UI**: Beautiful dark-themed interface with smooth animations
- **📱 Responsive Design**: Works seamlessly on desktop and mobile devices

## 🛠️ Tech Stack

### Backend
- **Flask** - Python web framework
- **Google Gemini 2.5 Pro** - Advanced AI model for business analysis
- **Flask-CORS** - Cross-origin resource sharing
- **python-dotenv** - Environment variable management

### Frontend
- **Vanilla JavaScript** - No framework dependencies
- **Chart.js** - Interactive data visualizations
- **CSS3** - Modern styling with animations
- **LocalStorage** - Client-side chat persistence

## 📋 Prerequisites

- Python 3.9 or higher
- Google Gemini API key ([Get one here](https://aistudio.google.com/app/apikey))
- Modern web browser

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/AI-Business-Idea-Market-Analyzer.git
cd AI-Business-Idea-Market-Analyzer
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory:

```env
GOOGLE_API_KEY=your_gemini_api_key_here
```

**Important:** 
- Don't commit this file to Git (add to `.gitignore`)
- For Vercel deployment, use Vercel's Environment Variables dashboard instead
- Get your API key from [Google AI Studio](https://aistudio.google.com/app/apikey)

### 4. Run the Application

```bash
python chat.py
```

The application will start on `http://localhost:5000`

## 🌐 Deployment to Vercel

### Quick Deploy

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/AI-Business-Idea-Market-Analyzer)

### Manual Deployment

#### 1. Install Vercel CLI (Optional)

```bash
npm install -g vercel
```

#### 2. Configure Environment Variables in Vercel

**Important:** You must add your API key in Vercel's dashboard:

1. Go to your Vercel project dashboard
2. Navigate to **Settings** → **Environment Variables**
3. Add the following variable:
   - **Name:** `GOOGLE_API_KEY`
   - **Value:** Your Google Gemini API key from [aistudio.google.com](https://aistudio.google.com/app/apikey)
   - **Environment:** Production, Preview, and Development

![Vercel Environment Variables](https://vercel.com/_next/image?url=https%3A%2F%2Fassets.vercel.com%2Fimage%2Fupload%2Fcontentful%2Fimage%2Fe5382hct74si%2F5XmNFtVAKwOYCEqOaKwaq8%2F3f6b5f1e8a0d8e5a5e5e5e5e5e5e5e5e%2Fenv-vars.png&w=3840&q=75&dpl=dpl_BHHvLy6w5YTmXeXRJYKyRq8WGN1z)

#### 3. Deploy via GitHub (Recommended)

1. Push your code to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Click "Import Project"
4. Select your GitHub repository
5. Vercel will automatically detect the `vercel.json` configuration
6. Add environment variables (if not already added)
7. Click "Deploy"

#### 4. Deploy via CLI

```bash
# Login to Vercel
vercel login

# Deploy to production
vercel --prod
```

#### 5. Verify Deployment

After deployment, visit your Vercel URL and check:
- ✅ API Status shows "Connected" in the header
- ✅ Chat functionality works
- ✅ File upload works

**The `vercel.json` configuration automatically handles:**
- Routing between Flask API (`/api/*`) and static frontend
- Python runtime configuration
- Static file serving

## 📁 Project Structure

```
AI-Business-Idea-Market-Analyzer/
├── api/
│   └── chat.py              # Flask backend API
├── frontend/
│   ├── index.html           # Main HTML structure
│   ├── styles.css           # Styling and animations
│   └── app.js               # Frontend logic and API calls
├── requirements.txt         # Python dependencies
├── vercel.json             # Vercel deployment config
├── .env                    # Environment variables (not committed)
└── README.md               # Project documentation
```

## 💻 Usage

### Starting a Conversation

1. Open the application in your browser
2. Type your business question in the input field
3. Press Enter or click the send button
4. Receive AI-powered insights and recommendations

### Example Prompts

- "Generate a business idea for sustainable fashion"
- "Analyze the market potential for AI-powered education tools"
- "Create a financial projection for a SaaS startup"
- "What are the latest trends in e-commerce?"
- "Develop a marketing strategy for a mobile app"

### Uploading Data Files

1. Click the "Upload File" button in the sidebar
2. Select a CSV, TXT, or JSON file (max 5MB)
3. Receive automated analysis with:
   - Key metrics summary
   - Trend analysis
   - Performance insights
   - Actionable recommendations
   - Visual charts (for numeric data)

### Managing Chat History

- **New Chat**: Click "New Chat" button to start fresh
- **Load Previous Chat**: Click any chat in the history sidebar
- **Auto-Save**: Conversations are automatically saved to browser storage


