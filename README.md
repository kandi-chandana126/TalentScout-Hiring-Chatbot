# TalentScout-Hiring-Chatbot
# TalentScout: Intelligent Hiring Assistant

**TalentScout** is an intelligent recruitment assistant designed to streamline the initial candidate screening process for a fictional recruitment agency specializing in technology placements. The chatbot collects essential candidate details, generates technical questions based on the candidate’s declared tech stack, and assesses their proficiency in each area. Leveraging **Large Language Models (LLMs)**, TalentScout provides an efficient and user-friendly experience for both recruiters and candidates.

## Project Overview

TalentScout automates the early stages of candidate recruitment by:
- Gathering vital candidate information (e.g., name, contact details, years of experience).
- Asking candidates about their tech stack (programming languages, frameworks, tools).
- Generating relevant technical questions tailored to the candidate’s skill set.
- Ensuring a smooth, context-aware conversation throughout the process.
- Gracefully concluding the conversation, providing information about next steps.

By leveraging the power of **LLMs** and **Streamlit**, TalentScout allows for efficient and personalized technical assessments, offering a seamless experience for both candidates and recruiters.

### Usage Guide
Launch the Application: Run the Streamlit app as mentioned above.
Input Candidate Information: Upon starting the conversation, the chatbot will ask for candidate details (e.g., name, contact info, years of experience).
Declare Tech Stack: The candidate will specify their proficiency in programming languages, frameworks, and tools.
Generate Technical Questions: Based on the provided tech stack, TalentScout will generate tailored technical questions to evaluate the candidate's skills.
End of Session: The chatbot will conclude the session and inform the candidate of the next steps in the recruitment process.

### Technical Details
Libraries Used:
Streamlit: For the frontend interface, making the app interactive and easy to use.
Transformers (Hugging Face): For utilizing pre-trained LLMs like GPT-3/4 to generate technical questions.
Python: The primary programming language used for backend logic, including data handling and chatbot responses.
Other dependencies: pandas, requests (for API calls), and any other libraries for auxiliary functions.

### Model Details:
The chatbot uses pre-trained models (e.g., GPT-3/4) to dynamically generate technical questions based on the tech stack provided by candidates. These models are fine-tuned with custom prompts to ensure that the questions are relevant to the specific technologies mentioned by the candidate.

### Architectural Decisions:
Streamlit Frontend: A simple, interactive UI was created using Streamlit, allowing users to provide inputs and interact with the chatbot.
Session Management: Streamlit’s session_state is used to store the user’s inputs and track conversation flow.
LLM Integration: The chatbot communicates with a pre-trained LLM to generate questions based on the candidate’s input.

### Prompt Design
Information Gathering:
Prompts were designed to gather the following candidate information:

Full Name
Contact Details (Email, Phone Number)
Years of Experience
Desired Position(s)
Current Location
Tech Stack (Languages, Frameworks, Databases, Tools)

### Challenges & Solutions
1. Context Management:
Maintaining context during the conversation was a challenge, especially when handling follow-up questions. The solution was to use Streamlit's session_state to store the user’s inputs and track conversation flow.

2. Generating Relevant Questions:
Generating specific and relevant technical questions for various tech stacks was tricky. We overcame this challenge by carefully crafting prompts for each technology stack (e.g., Python, JavaScript, React), ensuring that the LLM understood the nuances of each technology.

3. Handling Unexpected Inputs:
Handling user inputs that did not align with expected formats was another challenge. To solve this, we implemented fallback mechanisms that prompt the candidate to re-enter information in a clearer manner, without deviating from the hiring purpose.

4. Ensuring Data Privacy:
Since the app collects sensitive candidate information, we ensured that all data is anonymized and simulated during testing to comply with privacy standards (e.g., GDPR).

## Installation Instructions

Follow these steps to set up and run **TalentScout** locally:

### Step 1: Clone the Repository
Clone the project repository from GitHub:
```bash
git clone https://github.com/your-username/talentscout.git
cd talentscout



 
