# 🚀 Project Name

## 📌 Table of Contents
- [Introduction](#introduction)
- [Demo](#demo)
- [Inspiration](#inspiration)
- [What It Does](#what-it-does)
- [How We Built It](#how-we-built-it)
- [Challenges We Faced](#challenges-we-faced)
- [How to Run](#how-to-run)
- [Tech Stack](#tech-stack)
- [Team](#team)

---

## 🎯 Introduction
* Automated Ticket assignment system

   Everyday platform support team gets dump of csv files for open tickets. They have to manually read the ticker descriptions and assign to respective agents. To reduce this manual task we created automated ticket       
   assignment system where team will upload the csv file. It will automatically categorise the ticket (ticket is based on network/hardware/splunk issues) and assign to the agent

* Automated Platform Support chatbot  (Main Application)

   When platform support agent is assigned to a ticket, he/she has to go through many documents and many primary scripts they have to run for troubleshooting. We have automated this process. Platform support agent can 
   check what is the resolution for this type of ticket from earlier tickets csv dataset. Along with that platform support person can run the script from chatbot itself, no need to manually go diffrent places are check the 
   issue. Along with that they will get suggestions from what troubleshooting document we have provided/loaded in our llm

## 🎥 Demo
🔗 [Live Demo](#) (if applicable)  
📹 [Video Demo](#) 
   * Demo is uploaded inside https://github.com/ewfx/gaipl-best5/tree/main/artifacts/demo
🖼️ Screenshots:

![Screenshot 1](link-to-image)

## 💡 Inspiration
What inspired you to create this project? Describe the problem you're solving.

## ⚙️ What It Does
Explain the key features and functionalities of your project.

## 🛠️ How We Built It
The techstack what we used in this project are:
TextLoader, UnstructuredFileLoader and CSVLoader to load our internal throubleshooting/F&Q documents
OpenAI embedding - for text similarity, classification, recommendation
langchain
vectordb - FAISS, to load the document with embedding for personalised recommendation of tickets
LLM with model GPT-4 (as mentioned in problem statement)
RAG based qa chain - For retriving a user query from vector db. To retrive relevant documents or text chunks, which serve as context for the LLM.

## 🚧 Challenges We Faced
Describe the major technical or non-technical challenges your team encountered.

## 🏃 How to Run
1. Clone the repository  
   ```sh
   git clone https://github.com/ewfx/gaipl-best5.git
   ```
2. Install dependencies  
   ```sh
   pip install -r requirements.txt 
   ```
3. Create .env file to provide OPENAI_API_KEY 
   ```sh
   pip install -r requirements.txt 
   ```
4. Run the project  
   ```sh
   streamlit run .\code\src\ticketassignment.py
   streamlit run .\code\src\platformsupport.py   (This is the main application)
   ```

## 🏗️ Tech Stack
- 🔹 Frontend: Streamlit
- 🔹 Backend: python
- 🔹 Database: vectordb for RAG based solution
- 🔹 Other: OpenAI API 

## 👥 Team
- **Your Name** - [GitHub](#) | [LinkedIn](#)
- **Teammate 2** - [GitHub](#) | [LinkedIn](#)
