# AI Market Research Agent

An autonomous multi-agent system that researches AI industry trends and generates engaging blog posts using CrewAI.

## Description

This project uses CrewAI to orchestrate two AI agents that work together to research and write about AI industry trends:

1. **Market Researcher Agent** - Searches the web using Serper to find the latest AI trends from credible sources (IBM, McKinsey, Stanford, etc.)
2. **Content Writer Agent** - Transforms research findings into compelling, reader-friendly blog posts

The agents collaborate sequentially: the researcher gathers and analyzes data, then passes findings to the writer who creates the final blog post.

## Key Features

- Autonomous web research using Serper search tool
- Multi-agent collaboration with defined roles and goals
- Automatic source credibility assessment
- Theme-based content organization
- Generates publication-ready markdown blog posts

## Technologies Used

- **CrewAI** - Multi-agent orchestration framework
- **Gemini 2.5 Flash** - LLM for agent intelligence
- **Serper** - Web search API
- **LangChain** - Google Generative AI integration

## How It Works

1. Market Researcher agent searches for latest AI trends
2. Agent evaluates source credibility (prioritizing IBM, McKinsey, Stanford)
3. Researcher extracts key findings from each source
4. Findings are organized into themes
5. Writer agent creates an engaging blog post
6. Output is saved as a markdown file

## Sample Output Topics

Based on the included example, the system can identify and write about:

- Generative AI adoption in business
- Multimodal AI and Small Language Models
- Agentic AI systems
- AI integration across organizations
- Ethical AI and governance

## Setup

1. Install dependencies:
```bash
pip install crewai crewai-tools langchain-google-genai
```

2. Set up API keys:
   - Google API key (for Gemini)
   - Serper API key (for web search)

3. Run the Jupyter notebook to execute the agent workflow

## Files

- `Day19_autonomous_market_analyst_AIagents.ipynb` - Main notebook with agent definitions and workflow
- `blog_post.md` - Example output blog post
- `Output.txt` - Execution flow documentation

## License

This project is part of an AI agents learning series.
