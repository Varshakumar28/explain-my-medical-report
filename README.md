# explain-my-medical-report

1. Overview   
Explain My Report is an AI-based web application I developed to simplify complex medical documents into plain, easy-to-understand language using Small Language Models (SLMs).
This project demonstrates how modern language models can be applied to solve real-world communication problems, especially those involving accessibility and comprehension of medical, legal, or research reports by non-experts.
It served as my first hands-on experience in building a complete AI workflow — from data extraction to model interaction and web deployment — all running locally on CPU without the need for GPUs.

2. Problem Statement
Medical and research reports are typically written in domain-specific or technical language, making them difficult for patients and non-specialists to interpret.
This communication barrier between healthcare professionals and patients can lead to confusion, anxiety, and misinterpretation of important findings.
Objective
To develop a lightweight, CPU-deployable web application capable of:
•	Automatically reading medical report PDFs
•	Generating simplified summaries in plain English
•	Delivering accessible explanations without compromising on factual accuracy

3. Proposed Solution
The application enables users to upload a medical PDF report, extract the text, and process it through a Small Language Model (such as Phi-3-Mini or Mistral-7B).
The model is prompted to rewrite the extracted report in non-technical, patient-friendly language.
Workflow:
- Upload the medical report (PDF).
- Extract text using PyPDF2.
- Process the extracted text through an SLM with a prompt like “Explain this for a non-expert.”
- Display the simplified explanation in a Gradio web interface.
   
4. Skills Developed
During this project, I strengthened both my technical implementation and conceptual understanding of modern AI tools and workflows.
Skill Area	Description
Model Integration	Running and managing SLMs such as Phi-3-Mini and Mistral-7B using transformers and ollama.
Prompt Engineering	Designing prompts to guide tone, structure, and depth of model explanations.
Web Interface Development	Building interactive AI interfaces with Gradio for user-friendly experiences.
PDF Data Handling	Extracting, cleaning, and preparing text from PDF medical reports using PyPDF2.

5. Tools and Technologies Used
Tool / Library	Purpose
- Gradio	- Creates a web interface for seamless interaction between users and the AI model.
- Transformers (Hugging Face) - Loads and manages pretrained small language models.
- PyTorch (Torch)	- Serves as the underlying framework for model inference and computation.
- PyPDF2	- Handles reading and text extraction from uploaded PDF documents.

6. Implementation Summary
    Core Steps
    - Model Loading - Load a pretrained model (e.g., microsoft/phi-2) using the transformers library.
    - Text Extraction - Use PyPDF2 to extract text content from the uploaded PDF report.
    - Prompt Generation - Construct a prompt such as: “Explain this medical report in simple, patient-friendly language.”
    - Text Generation - Pass the prompt through the loaded model to generate a simplified explanation.
    - Output Display - Display the generated explanation inside a Gradio text box with scrollable output.

7. Expected Output
Input (Original Text from PDF)	Simplified Output (Model Response)
- “Mild cardiomegaly noted. No pleural effusion.”
    O/P - “Your heart is slightly larger than normal, but there’s no fluid around your lungs. Overall, this is a normal chest X-ray.”
 - “Small renal calculi observed in both kidneys.”
  O/P - “There are small kidney stones in both kidneys, but they are not causing any blockage.”

8. Key Learnings
  Through this project, I learnt how to:
  - Build and deploy a functional AI web app using Gradio.
  -	Run Small Language Models efficiently on CPU systems without GPUs.
  -	Perform prompt-driven reasoning for simplifying domain-specific text.
  -	Connect real-world data (medical reports) with language model capabilities.
  This hands-on work strengthened my foundation in applied AI, model integration, and user-facing AI workflows.

# Conclusion
Explain My Report illustrates a practical, real-world application of Small Language Models in improving the accessibility of technical information.
By combining language modeling, PDF parsing, and user interface design, the system bridges the communication gap between complex medical data and patient understanding.
This project has served as a foundational learning milestone for me — helping me understand how AI models can be integrated, tuned, and delivered as user-focused products.


