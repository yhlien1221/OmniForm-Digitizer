# OmniForm-Digitizer: From Paper to Database

An intuitive, AI-powered tool designed to bridge the gap between physical paperwork and digital efficiency. This application transforms messy, handwritten forms into organized digital data instantly, saving hours of manual entry. 

By combining the intelligence of **Google Gemini 1.5** with a user-friendly **Streamlit** interface, this project provides a seamless experience for Optical Character Recognition (OCR) and automated data extraction.

## Why This Matters?

Manual data entry is slow and prone to human error. This tool was built to:
* **Save Time**: Convert physical records to digital spreadsheets in seconds.
* **Ensure Accuracy**: Uses advanced AI to read handwriting that traditional scanners often miss.
* **Empower Users**: Designed with a simple "Human-in-the-Loop" workflow, allowing anyone to review and edit data before it’s saved.

---

## Key Features

* **Intelligent Schema Detection**: Automatically identifies all form labels and fields from an image using Large Multimodal Models (LMMs).
* **Selective Extraction**: Allows users to filter and choose only specific fields of interest, reducing data noise.
* **Human-in-the-Loop (HITL)**: Includes an editable data preview stage to ensure 100% accuracy before committing to the database.
* **Master Database Management**: Aggregates data from multiple forms into a single view with one-click CSV export functionality.
* **Cloud-Ready Deployment**: Pre-configured for Google Colab with `ngrok` tunneling for easy external access.

---

## Tech Stack

* **Core Logic**: Python
* **AI Engine**: Google Gemini 1.5 (Pro/Flash)
* **Frontend**: Streamlit (Interactive UI)
* **Data Handling**: Pandas (Master Database & CSV Export)
* **Networking**: Pyngrok (Secure Tunneling)

---

## The 4-Step Precision Pipeline

1.  **Scan**: Upload an image. The AI scans the document to "understand" the layout and list all available fields.
2.  **Filter**: Select only the specific data points you need from the detected list.
3.  **Extract**: The AI performs targeted extraction on handwritten text for the chosen fields.
4.  **Commit**: Review the extracted data in an editable table. If it looks good, save it to the permanent Master Database.

---

## Setup & Installation

### Prerequisites
* A Google Gemini API Key.
* An ngrok Auth Token (for Colab deployment).

### Local Execution
1.  **Install dependencies**:
    ```bash
    pip install streamlit google-generativeai pandas pillow pyngrok
    ```
2.  **Configure API Keys**:
    Replace `API_KEY` and `ngrok_auth_token` in the script with your credentials.
3.  **Launch the App**:
    ```bash
    streamlit run app.py
    ```

---

## Why This Project?

Manual data entry is prone to error and incredibly time-consuming. This tool demonstrates a modern approach to **Automated Document Processing (ADP)**. By combining the flexibility of Generative AI with a structured verification workflow, it ensures that the speed of AI is balanced with the reliability of human oversight.

---

## Contact
Feel free to reach out if you have questions about the architecture or implementation of this project!

**YU-HUI LIEN** [https://www.linkedin.com/in/yu-hui-lien/]