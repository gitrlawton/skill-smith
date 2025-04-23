# Career Compass: AI-Powered Career Gap Analyzer

## Overview

This GenAI project aims to assist students and professionals in understanding how to bridge the gap between their current experience and desired roles using generative AI. The project analyzes user resumes and provides personalized career transition roadmaps.

This project consists of a Jupyter Notebook where the generative AI model is prompted with the user's resume and their desired role in their desired field. The notebook displays a structured output that provides a detailed career plan, including transferable skills, missing skills, learning resources, and recommended certifications.

The notebook utilizes the Google GenAI API and Gemini Flash 2.0 to analyze resumes and generate actionable insights.

## Features

- **Resume Analysis**: Users can input their current resume, and the AI will extract transferable skills and identify gaps.
- **Personalized Career Roadmap**: The application generates a structured career plan tailored to the user's target role and sector.
- **Learning Resources**: Users receive recommendations for online courses and certifications to fill their skill gaps.
- **Intermediate Roles**: The roadmap includes suggested intermediate job titles to help users transition effectively.
- **Structured Output**: The results are formatted in a machine-readable JSON schema for easy integration with other applications.

## Installation

To set up the project, ensure you have Python installed on your machine. Then, follow these steps:

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Create a virtual environment:

   ```bash
   python -m venv .venv
   ```

3. Activate the virtual environment:

   - On Windows (using Command Prompt):
     ```bash
     .venv\Scripts\activate
     ```
   - On Windows (using Git Bash):
     ```bash
     source .venv/Scripts/activate
     ```
   - On macOS/Linux:
     ```bash
     source .venv/bin/activate
     ```

4. Create a `.env` file in the root directory and add your API keys:

   ```plaintext
   GEMINI_API_KEY=your_gemini_api_key
   ```

5. Save a copy of your resume as `my_resume.pdf` and place it in the root directory of the project.

6. Specify your desired role and sector in Cell 4.

7. Run the notebook.

## Usage

1. Run all of the cells in `CareerCompass.ipynb`, in order. This will install and load the necessary libraries, set the API key, and process the user's resume to generate a career plan.

2. Ensure your resume is named `my_resume.pdf` and is located in the same directory as the notebook.

3. The notebook will output a detailed career transition plan, including skills to learn and recommended resources.

## File Descriptions

- **CareerCompass.ipynb**: Jupyter notebook containing the code for analyzing resumes and generating career plans.

## Dependencies

- **Python**: The programming language used for this project.
- **httpx**: For making HTTP requests to the Google GenAI API.
- **dotenv**: For loading environment variables from a `.env` file.
- **Jupyter**: For running the Jupyter Notebook used to analyze resumes and generate career plans.
- **Google GenAI SDK**: For providing the API used to analyze resumes and generate personalized career insights.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any suggestions or improvements.
