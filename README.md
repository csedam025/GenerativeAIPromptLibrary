# Generative AI Prompt Library
This is a **Work-In-Progress** library of master/system prompts co-authored by myself and FREE artificial intelligence platforms. The purpose of this collection is to help inform anyone interested in leveraging these tools to better understand how to generate detailed and actionable responses from services like ChatGPT, Gemini, and more. These skills can be used across all Large Language Model (LLM) services as of this writing.


## Step 1: Understanding AI Response Frameworks
This sounds more complicated than it is. Simply put, a response framework is a speech pattern. If you do not tell the chatbot how it should speak to you, then you will get a different type of response every time you engage with it. 

Before giving it a task to work on, define how it should present its answers to you.

### Summary Table of AI Prompt Frameworks

| Framework Acronym  | Full Name | Use Case | Complexity |
| ------------- | ------------- | ------------- | ------------- | 
| RTF	Role  | Role, Task, Format  | Everyday tasks and simple requests. | Low | 
| RISEN	Role  | Role, Input, Steps, Expectation, Narrowing  | Detailed workflows, technical SOPs, and multi-step processes. | Medium |
| CO-STAR  | Context, Objective, Style, Tone, Audience, Response | Marketing copy, creative writing, and brand-aligned content. | High |
| BAB  | Before, After, Bridge | Strategy planning, problem-solving, and sales pitches. | Medium |
| CARE  | Context, Action, Result, Example  | Professional reporting, case studies, and executive summaries. | Medium |
| CREATE  | Character, Request, Examples, Adjustments, Type, Extras | Highly customized outputs requiring specific styles or "no-go" zones. | High |
| TAG  | Task, Action, Goal  | Goal-oriented management tasks and clear project definitions. | Low | 

###  Framework Explanation

1. RTF (The Essentials)

This is the "bread and butter" of prompting. It’s perfect for when you need a fast result without overthinking the structure.

    Example:
    
    Act as a Social Media Manager (Role).
    
    Write three captions for a new coffee blend (Task).
    
    Present them as a numbered list (Format).

2. RISEN (The Workflow Specialist)

When a task has multiple moving parts, RISEN prevents the AI from skipping steps.

    Example:
    
    Role: Expert Data Analyst

    Input: The attached CSV of Q1 sales.

    Steps:
    1.) Identify top 3 products. 
    2.) Calculate growth %. 
    3.) Predict Q2.

    Expectation: A professional summary table.

    Narrowing: Focus only on North American regions; ignore returns.

3. BAB (The Persuasion Framework)

This is a storytelling framework used to bridge the gap between a problem and a solution.

    Example:
    
    Before: Our team spends 5 hours a day on manual data entry.

    After: We want to automate this to under 30 minutes.

    Bridge: Write a proposal for an automated Python script that integrates with our CRM.

4. CO-STAR (The Professional standard)

Used heavily in corporate and creative environments to ensure the AI "speaks" the right language to the right people. It emphasizes Tone and Audience to avoid the "robotic" feel of standard AI responses.

    Example: 
    
    "Would you like me to take a specific task you're working on and draft a summarized response email to a supervisor?"


## Step 2: Building a "Role"
The goal here is to construct a prompt that pre-defines all the parameters the chatbot is required to use when generating its response. How we go about this is important because you'll not only be defining its "Personality", but also its "Experience-Level". There is plenty of documentation surrounding this online, but often the simplest path is just asking the chatbot what information it needs you to provide as each platform is slightly different.

I will outline a method of doing this below.

    1.) Open any GenAI service chatbot. (ChatGPT, Gemini, Claude, etc.)

    2.) Type in something along the lines of: "I would like to create a master prompt for the role of [INSERT ROLE]. What information do you need me to provide? Use [INSERT FRAMEWORK]"
          
          Role Examples: Senior Advertising Consultant, Expert Real Estate Agent, Junior Programmer, etc.
          
          Framework Examples: RTF, CO-STAR, TAG, etc.

    3.) Copy/Paste its response into a text document and answer each question as best you can.

    4.) Copy/Paste all the text within your answer document back into the chatbot.

    5.) Repeat this process until no further revisions are nessessary.

    6.) Tell the chatbot to download the current "role" and its parameters into a file for future use. (PDF, Text doc, etc.)

**Note:** I used the exact method described above to generate the GeminiSystemPromptSeniorAIPromptingV1.txt file using Gemini 3 Flash.

## Step 3: Testing the Role
At this point, it would be wise to thoroughly test the prompts generated from this new role as it may provide unexpected answers that will need to be addressed before live implementation. 

A simple way to do this would be:

    1.) Open a new session with any GenAI service chatbot. (ChatGPT, Gemini, Claude, etc.)
    
    2.) Upload the role file into the chatbot if supported, ortherwise copy/paste the text into it.
    
    3.) Start asking it to generate prompts to accomplish a task.

        Task Example - Role = Expert Real Estate Agent: Generate a prompt to scan all major property listing websites for three bedroom houses in zipcode 32789 with rent under $2,500 a month posted within the last week and provide sources.

        Task Example - Role = Senior Advertising Consultant: Generate a prompt to outline modern advertising strategies to promote a new menu item.

    
    4.) Adjust the generated prompts if needed, then execute them to review the results.

**Note:** If you're having to repeatedly include more information to get the desired result, make a note of the type of information manually being adjusted and update the role prompt to include this type of data analysis at the start to save time.
  
## Step 4: Review Additional Resources
Once you understand how these roles work, I would recommend reviewing how large corporations like Google compose their prompts, as they're not as complex as you'd imagine.

This link leads to a crowd sourced repository of some leaked system prompts used across the biggest names in AI development: https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools
