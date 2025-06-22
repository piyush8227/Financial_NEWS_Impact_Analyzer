# Financial_NEWS_Impact_Analyzer

## Project Directory Structure

financial-news-impact-analyzer/
│
├── agents/                        # All your agent logic goes here
│   ├── ingestion_agent.py         # Fetch news articles
│   ├── entity_recognition_agent.py# Extract company/ticker names
│   ├── sentiment_agent.py         # Analyze sentiment, output score
│   ├── impact_score_agent.py      # Calculate impact from sentiment
│   ├── evaluation_agent.py        # Align with price, compute metrics
│   └── report_agent.py            # Export structured output/logs
│
├── prompts/                       # Prompt templates & versions
│   ├── sentiment_prompt.txt
│   └── entity_extraction_prompt.txt
│
├── data/                          # Input/output & intermediate files
│   ├── raw_news/                  # Raw input data
│   ├── enriched_news/            # Parsed + sentiment/impact
│   └── backtest_results/         # Evaluation metrics
│
├── notebooks/                     # Jupyter notebooks for experimentation
│   └── backtest_exploration.ipynb
│
├── tests/                         # Basic unit & integration tests
│   └── test_sentiment_agent.py
│
├── utils/                         # Helper functions/modules
│   ├── logger.py
│   └── price_data_fetcher.py
│
├── ai_chat_history.txt            # Conversation history (auto-logged)
│
├── main.py                        # Entrypoint to run full pipeline
├── requirements.txt               # Python package dependencies
├── README.md                      # Your project overview + setup
└── docs/                          # Iteration notes, agent design, etc.
    ├── design.md
    ├── prompt_iterations.md
    └── failures_learnings.md
