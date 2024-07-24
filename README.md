# Customer Feedback Analysis using Agents

This repository contains a script that automates the collection, analysis, and reporting of customer feedback for the AirPods Pro using the OpenAGI framework. The script is designed to be interactive, with human intervention to ensure more accurate data collection and analysis.

## Overview

The primary goal of this project is to automate the process of gathering and analyzing customer feedback for AirPods Pro from various online platforms, and then generate a comprehensive report based on this analysis. The process is broken down into several key steps, managed by a multi-agent architecture within the OpenAGI framework:

1.  **Installation and Setup**: The script installs and configures necessary packages, including OpenAGI and an OpenAI API key.
2.  **API Configuration**: The script prompts the user to enter their OpenAI API key, which is required for accessing language model functionalities.
3.  **Large Language Model Configuration**: The script configures the OpenAI language model to handle various tasks such as data collection, analysis, and report generation.
4.  **Multi-Agent Architecture**: The script defines multiple worker agents, each with a specific role:

*   **Feedback Collector**: This agent gathers customer feedback from online platforms such as social media, review sites, and forums. It focuses on identifying common themes and sentiments related to AirPods Pro.
*   **Data Analyst**: This agent analyzes the collected feedback to identify key trends, recurring issues, and overall customer sentiment. It uses statistical tools to quantify the data and provide actionable insights.
*   **Report Creator**: This agent develops a comprehensive customer feedback analysis report. It highlights key findings, trends, and recommendations for improving the AirPods Pro, ensuring the report is well-structured and visually appealing.

1.  **Admin Agent**: The Admin agent oversees the entire process, using a task planner to break down the main task into smaller, manageable tasks. It assigns these tasks to the appropriate worker agents and ensures they are completed efficiently.
2.  **Human Intervention**: A key feature of this project is the human intervention capability. The Admin agent is designed to interact with the user during execution, asking questions to gather more precise information. This interaction helps improve the accuracy and relevance of the data collected and analyzed.
3.  **Execution**: Once all configurations are set, the Admin agent runs the task of creating a customer feedback analysis report. It leverages the defined worker agents to collect data, analyze it, and generate a detailed report.
4.  **Output**: The final output is a comprehensive report that includes:

*   **Collected Feedback**: Reviews and feedback from specified online sources.
*   **Data Analysis**: Insights on key trends, recurring issues, and overall customer sentiment.
*   **Recommendations**: Actionable suggestions for improving the AirPods Pro based on the analysis.

### How It Works

1.  **Install and configure dependencies**: The script installs required packages and sets up the OpenAI API key.
2.  **Define and configure agents**: Workers (Feedback Collector, Data Analyst, Report Creator) and the Admin agent are configured with specific roles and actions.
3.  **Enable human intervention**: The Admin agent is set to interact with the user for more accurate data collection.
4.  **Run the script**: Execute the script to start the feedback analysis process.
5.  **Generate report**: The script outputs a detailed report with collected feedback, data analysis, and recommendations.

## Installation

### Prerequisites

* Python 3.6 or higher
* Google Colab or any notebook of choice
* OpenAI API Key

### Install Dependencies

Make sure to install the OpenAGI package:

pip install openagi

## Usage

1.  **Set Up Environment Variables**: The script requires your OpenAI API key to function. You will be prompted to enter your OpenAI key when you run the script.
2.  **Run the Script**: Execute the Jupyter notebook `customer_feedback_analysis.ipynb` to start the feedback analysis process.

### Human Intervention

The `admin` agent has human intervention enabled (`human_intervene=True`). This means that during the execution, the admin will ask the user questions to get more accurate answers and ensure the task is carried out effectively. For example, the admin may ask for specific online sources or time periods for collecting customer feedback.

### Sample Interaction

Agent: Could you specify the online sources from which I should collect the customer feedback for the AirPods Pro?
You: Collect it from reviews on online stores like Amazon and Flipkart.
Agent: Could you specify which online sources should be used to collect the customer feedback for AirPods Pro?
You: Amazon.
Agent: Could you specify which online sources should be used to collect the customer feedback for AirPods Pro, and if there is a specific time period from which the feedback should be gathered?
You: Check recent reviews from 3 months ago at max.

## Output

The script will generate a customer feedback analysis report for the AirPods Pro. The report will include:

1.  **Collected Feedback**: Reviews and feedback gathered from specified online sources.
2.  **Data Analysis**: Statistical analysis and insights on key trends, recurring issues, and overall sentiment.
3.  **Recommendations**: Actionable suggestions for improving the AirPods Pro based on the analysis.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

This project uses the OpenAGI framework. For more information, visit [openagi.aiplanet.com](https://openagi.aiplanet.com).
