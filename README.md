# AI-Powered Profile Analysis and Evaluation System

An intelligent web application for resume analysis, career guidance, and technical assessment using AI and machine learning.

## 🚀 Features

- **AI-Powered Resume Analysis** - Upload PDF resumes and get intelligent analysis
- **Career Advisor Chat** - Get personalized career advice using AI AGENT
- **Technical Assessments** - Skills testing with webcam monitoring
- **Role-Based Access** - Admin, HR, and Candidate dashboards
- **Application Tracking** - Monitor application status and progress
- **Analytics Dashboard** - Visual reports and statistics
- **Database Management** - SQLite database for data persistence

## 📋 Prerequisites

- **Python 3.8+** (3.11 recommended)
- **Git** (for cloning the repository)
- **Webcam** (for technical assessments)
- **Groq API Key** (for AI features)

## 🛠️ Installation

### You can download zip fie also in <>Code section

### Step 1: Clone the Repository

```bash
git clone <repository-url>

```

### Step 2: Set Up Virtual Environment

#### On Linux/macOS:
```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
source venv/bin/activate
```

#### On Windows:
```cmd
# Create virtual environment
python -m venv venv

# Activate virtual environment
venv\Scripts\activate
```

### Step 3: Install Dependencies

```bash
# Install required packages
pip install -r requirements.txt
```

### Step 4: Configure Environment

1. **Create Streamlit Secrets File:**

Create a file `.streamlit/secrets.toml` with your Groq API key:

```toml
GROQ_API_KEY = "your_groq_api_key_here"
```

Replace in  file `.env` with your Groq API key:

```toml
GROQ_API_KEY = "your_groq_api_key_here"
```
Replace in  file `app.py` with your MODEL ID
IN line 28 and 73

Same in `pages/test.py`with your MODEL ID
IN line 75
```toml
MIXTRAL_MODEL = "MODEL ID"
```

2. **Get Groq API Key:**
   - Visit [Groq Console](https://console.groq.com/)
   - Sign up/Login and create an API key
   - Replace `your_groq_api_key_here` with your actual API key

3. **Add available model::**
   - Visit [Groq Model](https://console.groq.com/docs/models)
   - Replace `your_MODEL_ID _here` with available MODEL ID

   
## 🚀 Running the Application

### Method 1: Using Streamlit Command

#### On Linux/macOS:
```bash
# Activate virtual environment
source venv/bin/activate

# Run the application
streamlit run app.py
```

#### On Windows:
```cmd
# Activate virtual environment
venv\Scripts\activate

# Run the application
streamlit run app.py
```

### Method 2: Using Python Module

#### On Linux/macOS:
```bash
# Activate virtual environment
source venv/bin/activate

# Run using python module
python3 -m streamlit run app.py
```

#### On Windows:
```cmd
# Activate virtual environment
venv\Scripts\activate

# Run using python module
python -m streamlit run app.py
```

### Method 3: Specify Custom Port

```bash
# Run on specific port (e.g., 8501)
streamlit run app.py --server.port 8501
```

## 🌐 Accessing the Application

Once the application is running, you can access it at:

- **Local URL:** `http://localhost:8501`
- **Network URL:** `http://your-ip-address:8501`

## 👥 User Roles

### 1. **Admin**
- Full system access
- Analytics dashboard
- User management
- Application oversight
- Initial id/pass is admin/admin123456

### 2. **HR**
- Candidate management
- Application review
- Assessment monitoring
- Notes and feedback
- Initial id/pass is hr/hr123456

### 3. **Candidate**
- Profile management
- Resume upload
- Application submission
- Technical assessments

## 📁 Project Structure

```
AI-Powered-Analytical-Profile-Analysis-And-Evaluation-System/
├── app.py                 # Main application file
├── auth.py               # Authentication module
├── database.py           # Database operations
├── requirements.txt      # Python dependencies
├── .streamlit/
│   └── secrets.toml     # API keys and secrets
├── uploads/
│   └── resumes/         # Uploaded resume files
├── data/
│   └── users.db         # SQLite database
└── README.md            # This file
```

## 🔧 Configuration Options

### Streamlit Configuration

You can customize the application by creating a `.streamlit/config.toml` file:

```toml
[server]
port = 8501
address = "localhost"
headless = true

[browser]
gatherUsageStats = false

[theme]
primaryColor = "#1E88E5"
backgroundColor = "#FFFFFF"
secondaryBackgroundColor = "#F0F2F6"
textColor = "#262730"
```

### Database Configuration

The application uses SQLite by default. The database file is automatically created at `data/users.db`.




## 📦 Dependencies

The application requires the following Python packages:

- `streamlit` - Web application framework
- `streamlit-extras` - Additional Streamlit components
- `python-dotenv` - Environment variable management
- `PyPDF2` - PDF processing
- `groq` - AI API client
- `scikit-learn` - Machine learning library
- `pandas` - Data manipulation
- `plotly` - Interactive visualizations
- `Pillow` - Image processing
- `mysql-connector-python` - Database connectivity

## 👥 My Team  

- **Aniruddha**  
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/aniruddhateware/)  
  [![GitHub](https://img.shields.io/badge/GitHub-black?style=for-the-badge&logo=github)](https://github.com/MasterMood)  

- **Renuka**  
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/renuka-siraskar-45159026a/)  
  [![GitHub](https://img.shields.io/badge/GitHub-black?style=for-the-badge&logo=github)](https://github.com/SiraskarRenuka)  

- **Shital**  
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/shital-deshpande-749ba2250/)  
  [![GitHub](https://img.shields.io/badge/GitHub-black?style=for-the-badge&logo=github)](https://github.com/shital21d)  

- **Anshul**  
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/anshulmehare0903/)




