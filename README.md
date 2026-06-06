# NLP Model Evaluation using Prompt Engineering

## Project Overview
This project evaluates the performance of multiple Large Language Models (LLMs) across different Natural Language Processing (NLP) tasks using Prompt Engineering techniques.

The study compares model outputs generated using Single-Step and Chain-of-Thought prompting strategies and evaluates them using both automated NLP metrics and human-centered quality measures.

## Objectives
- Compare the performance of different LLMs.
- Analyze the impact of prompt engineering techniques.
- Evaluate generated responses using NLP metrics.
- Measure qualitative aspects such as coherence, creativity, and logical consistency.

## Tasks Evaluated
1. Creative Writing
2. Code Generation
3. Summarization
4. Question Answering

## Prompting Techniques
- Single-Step Prompting
- Chain-of-Thought (CoT) Prompting

## Evaluation Metrics

### Automated Metrics
- BLEU Score
- ROUGE Score
- Task Success Rate

### Human Evaluation Metrics
- Coherence (1–5)
- Creativity (1–5)
- Logical Consistency (1–5)

## Dataset
The dataset contains:
- Task Type
- Model Name
- Prompt Type
- Input Prompt
- Generated Output
- Evaluation Scores

## Technologies Used
- Python
- Pandas
- NLTK
- ROUGE Score
- Hugging Face Datasets
- Google Colab

## Project Workflow
1. Generate prompts for multiple NLP tasks.
2. Apply Single-Step and Chain-of-Thought prompting.
3. Collect model outputs.
4. Evaluate outputs using BLEU and ROUGE.
5. Perform qualitative assessment.
6. Compare model performance.

## Results
The analysis demonstrates how different prompting strategies influence model performance across various NLP tasks. Chain-of-Thought prompting generally improves reasoning quality and logical consistency for complex tasks.

## Repository Structure
├── NLP Project.ipynb
├── updated_NLP.csv
├── README.md
└── Results/ (optional)

## Future Improvements
- Evaluate additional LLMs.
- Incorporate BERTScore and METEOR metrics.
- Create interactive dashboards for visualization.
- Automate evaluation pipelines.

## Author
Pavan Bathula
