# Documentation for Chatbot using ChatGPT4

## Overview

This Chatbot application leverages OpenAI's ChatGPT4 model to simulate an interview-style conversation. Its primary objective is to extract vital information from the user, essential for creating a LinkedIn profile. This chatbot uses a set of system prompts to guide the chatbot and produce deterministic responses. 

## Features

### 1. Interview-style Chat

The Chatbot initiates an interview-style conversation with the user. It asks a series of questions designed to glean essential information about the user's experience, qualifications, skills, and other relevant details. These details are crucial for constructing a professional LinkedIn profile.

**How to Use**:
- Launch the application. `streamlit run GUI.py`
- Engage with the chatbot and answer the questions as prompted.
- Ensure you provide accurate and comprehensive information for a more detailed profile.

### 2. LinkedIn Profile Builder

Based on the user's responses during the interview, the Chatbot processes this information to generate a LinkedIn profile. This feature helps users who are unsure about how to best present themselves on the platform or those looking for a quick way to get started.

**How to Use**:
- After completing the interview chat, use the sidebar option labeled "Create Profile."
- The Chatbot will then generate a LinkedIn profile based on the information provided during the chat.
- You can then download the profile using the "Download Profile" button.

### 3. Recommendations

To add value to the user's LinkedIn profile, the Chatbot provides recommendations on potential projects, studies, or other valuable additions that can enhance the profile's appeal. This feature offers users insights into areas they might not have considered and can make their profile stand out.

**How to Use**:
- Once the LinkedIn profile has been generated, the Chatbot will offer a series of recommendations.
- Consider incorporating these suggestions into your actual LinkedIn profile or using them as a basis for further professional development.

## Implementation

The Chatbot uses a combination of system prompts and user interactions to guide its responses. These prompts are stored in files like `System_prompts\Interview.md`, `System_prompts\Profilebuilder.md`, and `System_prompts\Suggestions.md`.

For a deterministic response from the ChatGPT4 model, the application sets the `temperature` parameter to 0 during interactions, ensuring that the model's output remains consistent across multiple sessions.

## Getting Started

1. **Environment Setup**:
   - Ensure you have the necessary libraries installed, including `streamlit`, `openai`, `dotenv`, among others.
   - Obtain an OpenAI API key and save it in a `.env` file under the variable `OPENAI_API_KEY`.
  
2. **Running the Application**:
   - Navigate to the directory containing the chatbot script.
   - Run the script using the command: `streamlit run GUI.py`
   - Follow the on-screen instructions to interact with the Chatbot.

