# **AI Resume Critiquer**

## **Features**
- Uploads resumes in a `pdf` or `txt` format
- Optional prompt input to filter feedback for specific job roles
- Automatic Text Extraction
    - `.txt` -> read directly with `.read()` and `.decode()`
    - `.pdf` -> parsed using **PyPDF2**
- Generates a customized analysis using the **OpenAI API**
- Clean, interactive interface powered by **Streamlit**

## **Tech Stack**
- **uv** → package management (installed Streamlit, OpenAI, python-dotenv, PyPDF2)
- **Streamlit** → web interface for uploading resumes and displaying results
- **PyPDF2** → PDF text extraction
- **python-dotenv** → secure environment variable management
- **OpenAI API** → AI-driven resume critique and role-specific feedback

## **How It Works**
1. Upload a `.pdf` or `.txt` resume
2. (Optional) Enter a prompt to tailor the analysis toward a specific job role
3. Resume text is extracted depending on file type
4. A prompt is constructed and sent to the **OpenAI API**
5. The AI-generated feedback is displayed on the **Streamlit** webpage
