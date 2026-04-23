
#### **Setup Instructions** 🛠️

Follow the steps below to set up and run the **Smart AI Resume Analyzer** on your local machine.

1. **Clone the repository:**

Open a terminal and run:

   ```bash
   git clone https://github.com/Hunterdii/resume-analyzer-ai.git
   cd Smart-AI-Resume-Analyzer
   ```

2. **Create a Virtual Environment(Optional)**

Set up a virtual environment to manage dependencies:

```bash
python -m venv venv
```

#### **Activate the Virtual Environment:**

- **Windows:**
  ```bash
  venv\Scripts\activate
  ```
- **MacOS & Linux:**
  ```bash
  source venv/bin/activate
  ```

3. **Install dependencies:**

Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

4. **Download the spaCy model:**

Ensure that the necessary NLP model is installed:

   ```bash
   python -m spacy download en_core_web_sm
   ```
   
``Congratulations 🥳😱 your set-up 👆 and installation is finished 🥳😱``


5. **Configure Environment Variables (Mandatory for AI-Analyzer Functionality):**

To enable access to the **Gemini API** used by the AI Resume Analyzer, you need to set up environment variables securely.

#### ✅ Step-by-Step:

1. **Create a `.env` file** inside the `utils/` directory.
2. **Paste your Google Gemini API key** in the following format:

#### 📄 Example content for `utils/.env`:
```env
GOOGLE_API_KEY=your_google_gemini_api_key
```

#### <img src="https://assets.codepen.io/1468070/Google+G+Icon.png" alt="Google LOGO" width="1.6%" /> Get your Gemini API Key:
Visit  **[Google AI Studio – Gemini API Access](https://aistudio.google.com/app/apikey)** 👉 Grab and use your **own API key** — Since Mine One Have Usage Limits.


6. **Run the application:**

Start the application using Streamlit:

   ```bash
   streamlit run app.py
   ```

<details>
  <summary>📁 Folder Structure After Adding <code>.env</code></summary>


### 🔹 Admin Panel Access:
   - The **Admin Section** will be visible **only after login**, right below the **Dashboard** section.

<!--### Deploy to Streamlit Cloud

1. Push your code to GitHub
2. Sign up for [Streamlit Cloud](https://streamlit.io/cloud)
3. Create a new app and connect it to your GitHub repository
4. Add your API keys as secrets in the Streamlit Cloud dashboard
5. Deploy the app

### Deploy with Docker

1. Build the Docker image:
   ```bash
   docker build -t smart-resume-analyzer .
   ```

2. Run the container:
   ```bash
   docker run -p 8501:8501 -e GOOGLE_API_KEY=your_key smart-resume-analyzer
   ```

## Project Structure

```
Smart-AI-Resume-Analyzer/
├── app.py                  # Main application file
├── config/                 # Configuration files
│   ├── courses.py          # Course recommendations
│   ├── database.py         # Database operations
│   └── job_roles.py        # Job role definitions
├── dashboard/              # Dashboard components
├── feedback/               # Feedback system
├── jobs/                   # Job search functionality
├── static/                 # Static assets
│   ├── css/                # CSS files
│   └── images/             # Image files
├── style/                  # Style definitions
├── templates/              # Resume templates
├── ui_components/          # UI components
├── utils/                  # Utility functions
│   ├── ai_resume_analyzer.py  # AI analysis logic
│   ├── resume_analyzer.py     # Standard analysis logic
│   └── resume_builder.py      # Resume builder logic
├── .env                    # Environment variables (not in git)
├── .gitignore              # Git ignore file
├── Dockerfile              # Docker configuration
├── LICENSE                 # License file
├── README.md               # This file
└── requirements.txt        # Python dependencies
```

