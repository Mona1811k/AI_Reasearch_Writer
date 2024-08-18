# AI_Reasearch_Writer

#Project Overview
This project is designed to automate the research and writing process using AI agents. The agents are created using the crewai framework and are tasked with researching and writing about specific topics related to technology, particularly focusing on uncovering and narrating groundbreaking innovations.

The project consists of the following main components:

#Agents:

newsresearcher: A senior researcher agent responsible for uncovering the latest technologies and trends within a given topic. The agent uses the ChatGoogleGenerativeAI model to perform its tasks and has the ability to delegate tasks.
news_writer: A writer agent tasked with composing engaging and accessible articles based on the research conducted. This agent also uses the ChatGoogleGenerativeAI model but is focused on creating content that is easy to understand and informative.
#Tasks:

research_task: A task that the newsresearcher agent handles, which involves identifying the next big trend in the provided topic. The output is a comprehensive 3-paragraph report.
writer_task: A task handled by the news_writer agent, which involves composing an insightful article based on the research findings. The output is a 4-paragraph article formatted in Markdown.
Crew:

The Crew consists of both the newsresearcher and news_writer agents. The tasks are executed in a sequential process, where the research is conducted first and then passed on to the writer for article creation.
Tools:

The project uses SerperDevTool, which is a custom tool that integrates with the Serper API for enhanced data retrieval and processing.
File Breakdown
agents.py: Defines the AI agents (newsresearcher and news_writer) and their respective roles, goals, and behaviors.
crew.py: Manages the orchestration of agents and tasks using the Crew class. It kicks off the process of task execution with the specified inputs.
tasks.py: Defines the specific tasks for the research and writing process, including the expected outputs and assigned agents.
tools.py: Handles the integration with external tools, particularly the Serper API, to aid in research tasks.
