# External Integration Project Progress Report (Crewai)

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
  - [Jupyter Notebook](#jupyter-notebook)
  - [Helper Functions](#helper-functions)
  - [Agents Configuration](#agents-configuration)
  - [Tasks Configuration](#tasks-configuration)
  - [Dependencies](#dependencies)
- [Installation](#installation)
- [Setup](#setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Overview
This project leverages the [Crewai framework](https://pypi.org/project/crewai/) to generate comprehensive progress reports by integrating external data from Trello. 
The solution is designed to automatically collect project data, analyze it for blockers and delays, and generate a detailed sprint report that includes:
- Sprint Overview
- Task Summary
- Identified Issues and Blockers
- Progress and Delays
- Team Performance Overview
- Action Items and Recommendations

## Project Structure
- **Jupyter Notebook**  
  `External_Integration_Project_Progress_Report(Crewai).ipynb`  
  Contains the main implementation and interactive examples.

- **Helper Functions**  
  `helper.py`  
  Includes utility functions for loading environment variables and retrieving API keys.

- **Agents Configuration**  
  `agents.yaml`  
  Defines the roles for:
  - **data_collection_agent**: Gathers project data from the Trello board.
  - **analysis_agent**: Analyzes collected data to identify progress issues and blockers.

- **Tasks Configuration**  
  `tasks.yaml`  
  Outlines the workflow tasks:
  - **data_collection**: Uses the Trello Data Fetcher tool to gather project data.
  - **data_analysis**: Processes the collected data to summarize project status.
  - **report_generation**: Compiles the analyzed data into a comprehensive sprint report in markdown format.

- **Dependencies**  
  `requirements.txt`  
  Lists the required Python packages and their versions:
  - crewai==0.75
  - crewai_tools==0.12.1

## Installation
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/External-Integration-Project-Progress-Report-Crewai.git
   cd External-Integration-Project-Progress-Report-Crewai

2. **Set Up a Virtual Environment:**
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```
3. **Install Dependencies:**
 ```bash
   pip install -r requirements.txt
```

## Setup
- Environment Variables:
Create a .env file in the root directory and add your API key:
```
OPENAI_API_KEY=your_openai_api_key_here
```
## Trello Integration:
- Ensure your Trello API settings are correctly configured if your project requires access to a Trello board.

  ![Uploading image.png…]()


 ## Usage
- **Interactive Development:**
Open and run the Jupyter Notebook External_Integration_Project_Progress_Report(Crewai).ipynb to interact with the project modules and view sample outputs.

- **Automated Workflow:**
- The project workflow includes:

**Data Collection:** 
- Automatically fetches project data from Trello.

**Data Analysis:**
- Processes and analyzes the collected data for key performance metrics.
  
**Report Generation:**
- Produces a detailed markdown report ready for review by the executive team.


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
