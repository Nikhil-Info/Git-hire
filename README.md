# GitHire - Profile Analyst

GitHire is an intelligent web application designed to help developers "hack the job market". By analyzing a user's GitHub profile, it identifies skill gaps and generates specific, hiring-ready coding project ideas tailored to demonstrate seniority and technical depth.

Powered by Google's Gemini 3 Flash model, GitHire goes beyond generic tutorials, offering architectural strategies and full implementation guides to help you build portfolio pieces that stand out to engineering managers.

## 🚀 Features

-   **Instant Profile Scanning**: Connects to the GitHub API to fetch repositories, top languages, and activity data.
-   **AI-Driven Gap Analysis**: Uses Gemini 3.0 logic to deduce your current skill level and find missing pieces in your stack (e.g., suggesting backend projects for frontend-heavy profiles).
-   **Hiring-Ready Suggestions**: Generates project ideas with a focus on business value, complexity, and learning outcomes.
-   **Immersive Guides**: Auto-generates comprehensive, step-by-step implementation guides for every suggestion, including code snippets and architecture breakdowns.
-   **Persistent State**: Saves your generated guides and progress locally so you can return to them later.
-   **Modern UI**: Features a glassmorphism design, dark/light mode, and smooth animations.

## 🛠️ Tech Stack

-   **Frontend**: React 19, TypeScript
-   **Styling**: Tailwind CSS (with custom animations and glass effects)
-   **AI Engine**: Google Gemini API (`@google/genai`) - specifically the `gemini-3-flash-preview` model.
-   **Routing**: React Router DOM (HashRouter for compatibility).
-   **Data Source**: GitHub REST API.

## 📦 Setup & Usage

1.  **Clone the repository**
2.  **Install dependencies**:
    ```bash
    npm install
    ```
3.  **Configure Environment**:
    You need a Google Gemini API Key.
    Create a `.env` file (or configure your environment variables) with:
    ```
    API_KEY=your_gemini_api_key_here
    ```
4.  **Run the application**:
    ```bash
    npm run dev
    ```

## 💡 How it works

1.  Enter a valid GitHub username.
2.  GitHire fetches public repository data (names, descriptions, languages, topics).
3.  This data is summarized and sent to Gemini with a prompt designed to act as a "Senior Engineering Manager".
4.  Gemini returns a candidate summary and 3 project suggestions.
5.  Clicking "Generate Guide" creates a deep-linkable page (e.g., `#/guide/custom-compiler`) with a full technical breakdown.

## Star History

[[![Star History Chart](https://api.star-history.com/svg?repos=Nikhil-Info/Git-hire.git&type=date&legend=top-left)](https://www.star-history.com/#Nikhil-Info/Git-hire.git&type=date&legend=top-left)](https://www.star-history.com/#Nikhil-Info/Git-hire.git&type=date&legend=top-left)

## 📝 License

MIT
