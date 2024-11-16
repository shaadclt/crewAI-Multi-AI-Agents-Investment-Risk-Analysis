# Using crewAI Multi AI Agents for Investment Risk Analysis

This project automates the process of monitoring market data, developing trading strategies, executing trades, and assessing risks using a team of specialized AI Agents from crewAI. Each agent is equipped with specific roles and goals, and they collaborate to optimize trading decisions and strategies. The project leverages the crewai library and langchain_community tools to facilitate communication and task management among the agents.

## Agents
### Data Analyst Agent
- Role: Monitor and analyze market data in real-time to identify trends and predict market movements.
- Goal: Provide critical insights for trading decisions.
- Specialization: Financial markets, statistical modeling, and machine learning.
- Tools: ScrapeWebsiteTool, SerperDevTool

### Trading Strategy Developer
- Role: Develop and test various trading strategies leveraging insights from the Data Analyst Agent.
- Goal: Formulate and optimize profitable and risk-averse trading strategies.
- Specialization: Financial markets, quantitative analysis.
- Tools: ScrapeWebsiteTool, SerperDevTool

### Trade Advisor
- Role: Recommend optimal trade execution strategies based on approved trading plans.
- Goal: Ensure trades are executed efficiently and aligned with the overall strategy.
- Specialization: Analysis of timing, price, and logistical details of potential trades.
- Tools: ScrapeWebsiteTool, SerperDevTool
  
### Risk Advisor
- Role: Evaluate and provide insights on the risks associated with potential trading activities.
- Goal: Deliver comprehensive risk analysis and recommend safeguards.
- Specialization: Risk assessment models, market dynamics.
- Tools: ScrapeWebsiteTool, SerperDevTool
  
## Tasks
### Data Analyst Agent: Analyze Market Data
- Description: Continuously monitor and analyze market data for the selected stock.
- Techniques: Statistical modeling, machine learning.
- Output: Generate insights and alerts regarding significant market opportunities or threats.
  
### Trading Strategy Agent: Develop Trading Strategies
- Description: Develop and refine trading strategies based on insights from the Data Analyst and user-defined risk tolerance.
- Considerations: User's risk tolerance, trading preferences.
- Output: A set of potential trading strategies aligned with the user's risk tolerance.

### Trade Advisor Agent: Plan Trade Execution
- Description: Analyze approved trading strategies to determine the optimal execution methods.
- Considerations: Current market conditions, pricing strategies.
- Output: Comprehensive execution plans detailing how and when to execute trades.

### Risk Advisor Agent: Assess Trading Risks
- Description: Evaluate the risks associated with the proposed trading strategies and execution plans.
- Output: A comprehensive risk analysis report with mitigation recommendations.

## Setup
1. Install Required Packages
```bash
pip install crewai==0.28.8 crewai_tools==0.1.6 langchain_community==0.0.29
```

2. Set Up API Keys
- Ensure you have the following API keys set up in your environment:
```bash
SERPER_API_KEY
OPENAI_API_KEY
```

3. Running the Project
- To execute the project, ensure all dependencies are installed, API keys are set, and agents are properly configured. Run all the tabs of the notebook one by one.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.

