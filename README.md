# CyanOracle
This is an AI tool to explore the Cyanotypes Creative Agency Circle content and to custom build educational pathways to meet learner goals. More information about the Cyanotypes projects is here https://cyanotypes.website/ 

## How do I use this tool?

The easiest way to try the tool out is to use one of the example instances listed here. Always be careful of the accuracy of the output. Changes in the LLM models that happen behind the scenes can cause the tool to start hallucinating quite wildly, we have seen this happen.  

Example instances:
 - Claude 3.5 Sonnet - https://claude.ai/project/3f78cfb5-9d4d-476f-b6ec-00789bc69ac2 
 - ChatGPT - https://chatgpt.com/g/g-eo4keBsHH-cyanoracle 
 - Argo - Available for Cyanotypes partners in the Argo Cyanotypes Workspace https://app.argo-g.pt/workspaces/4f12bb5e-e984-4afb-bc99-1271913e0592 

You can also recreate this tool using your preferred cloud based AI platform (e.g ChatGPT, Mistral, Claude, POE) or even run it locally on your own hardware if you know how to do that. All the necessary files, prompts and configuration parameters are included in this repository.

## Who is this tool for?

This tool is primarily for partners of the the Cyanotypes consortium but we are looking to widen the user base and use cases for the tool. Other users we are thinking of are:
 - Cyanotypes stakeholders who wish to explore the creative agency circle
 - Educational content designers who are building the next generation of courses for the creative industries
 - Higher education and VET institutions who are interested in offering their students more customised learning experiences
 - Learners who want to create a custom curriculum that meets their specific needs

## What can this tool do?

This tool is an AI agent that can explore the Cyanotypes creative agency circle content and identify relevant parts of the content given a user need. The creative agency circle contains five cluster areas, each of which has five competences, each of which have several learning outcomes. You can tell the AI you have a particular goal and it will find which learning outcomes are suitable for meeting the stated goal. If there are course modules or lessons (more are being developed) then it will ask you if you would like to see them.

The tool can take inputs from a defined persona. For example and Italian fashion design student that has the goal of being reday for business in a competitive environment or a Swedish games developer who needs to learn about collaborating across ecosystems. If you don't have a persona to work with the tool can generate one for you given zero or a few parameters.

### Some use cases
 - A student who wants to find specific learning opportunities to meet their identified goals
 - An educational institution administrator who want to offer custom tailored curricula to students
 - An educational content designer who wants to understand the necessary competences for the creative agency Circle
 - A policy maker who wants to explore the future skills needs for the creative industries
  

## How does this tool work?

This is a very simple AI tool that uses prompt engineering and simple Retrieval Augmented Generation to answer questions and make suggestions based on the creative agency circle developed by the Cyanotypes project. It presumes that the user will state some kind of need or goal for some type of persona. If you don't already have a persona in mind then it can create a fictional one for you based on the templates used in the cyanotypes development process. Once given an input it will search through a dataset of the creative agency circle competences, learning outcomes, and lessons (if those are available) and suggest a learning path that meets the expressed need. It will also provide some justification for the suggestions it makes. 

## How do I recreate this tool myself?
Using your AI tool of preference you can recreate this agent.
 1. Copy the 'cyanoracle prompt.txt' text into the agent instruction box
 2. Add the 'CyanOracle Creative Agency Circle.csv', 'CyanOracle Lessons clean.csv', and 'persona-template-schema-with-instructions.txt' into your agents' knowledge base or files.
 3. If your system uses additional parameters like temperature or setting token limits you can find our settings in the 'config.txt' file.

If you prefer to work with JSON then the data is also supplied in JSON format.  

## Can I contribute?

Yes! We are on a learning journey ourselves so any feedback or contributions are welcome. We particularly welcome ideas about how to refine the prompt and also how to best structure the data in the knowledge base for a more accurate and performant RAG pipeline.