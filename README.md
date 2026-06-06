# NLP Model Evaluation using Prompt Chaining: Claude vs Gemini

## Overview

This project investigates the impact of **Prompt Chaining** on the output quality of Large Language Models (LLMs). A comparative analysis was conducted using **Claude** and **Gemini** across four diverse NLP tasks: Creative Writing, Code Generation, Mathematical Reasoning, and Summarization.

The study evaluates whether breaking complex tasks into sequential prompts improves model performance compared to traditional single-prompt approaches. Performance was measured using both automated NLP metrics and human evaluation criteria.

---

## Project Objectives

* Evaluate the effectiveness of Prompt Chaining in improving LLM outputs.
* Compare the performance of Claude and Gemini across multiple NLP tasks.
* Measure improvements using quantitative and qualitative evaluation metrics.
* Identify task domains where Prompt Chaining provides the greatest benefits.

---

## Research Questions

1. Does Prompt Chaining improve output quality compared to Single Prompting?
2. Which model benefits more from Prompt Chaining?
3. How does Prompt Chaining affect reasoning, creativity, coherence, and task success?

---

## Tasks Evaluated

### Creative Writing

Generate engaging and coherent stories from writing prompts.

### Code Generation

Generate Python solutions from natural language programming problems.

### Mathematical Reasoning

Solve multi-step arithmetic and logical reasoning problems.

### Summarization

Generate concise summaries of long-form news articles.

---

## Datasets Used

| Task                   | Dataset                           |
| ---------------------- | --------------------------------- |
| Creative Writing       | Gryphe/ChatGPT-4o-Writing-Prompts |
| Code Generation        | OpenAI HumanEval                  |
| Mathematical Reasoning | GSM8K                             |
| Summarization          | CNN/DailyMail                     |

A total of 12 representative samples were selected (3 from each dataset), resulting in:

* 4 Tasks
* 3 Samples per Task
* 2 Models
* 2 Prompting Strategies

**Total Evaluations: 48**

---

## Prompting Techniques

### Single Prompt

A direct instruction asking the model to complete the task in one step.

Example:

```text
Write a short story about a scientist who discovers a hidden civilization beneath the ocean.
```

### Prompt Chaining

The task is broken into multiple sequential steps.

Example:

Step 1: Create a story outline.

Step 2: Expand the outline into a complete story.

This structured approach guides the model through planning and execution.

---

## Evaluation Metrics

### Automated Metrics

| Metric            | Purpose                                                |
| ----------------- | ------------------------------------------------------ |
| BLEU Score        | Measures output accuracy and n-gram overlap            |
| ROUGE-L Score     | Measures summary quality and content alignment         |
| Task Success Rate | Determines whether the task was completed successfully |

### Human Evaluation Metrics

| Metric              | Scale |
| ------------------- | ----- |
| Coherence           | 1–5   |
| Creativity          | 1–5   |
| Logical Consistency | 1–5   |

---

## Results

### Average Performance Across All Tasks

| Metric              | Single Prompt | Prompt Chaining | Improvement |
| ------------------- | ------------- | --------------- | ----------- |
| BLEU Score          | 0.62          | 0.71            | +0.09       |
| ROUGE-L Score       | 0.41          | 0.46            | +0.05       |
| Coherence           | 3.80          | 4.40            | +0.60       |
| Creativity          | 3.70          | 4.30            | +0.60       |
| Logical Consistency | 3.90          | 4.20            | +0.30       |
| Task Success Rate   | 67%           | 85%             | +18%        |

### Key Findings

* Prompt Chaining consistently improved output quality.
* The largest gains were observed in Mathematical Reasoning and Code Generation tasks.
* Claude achieved slightly better performance in reasoning-intensive and creative tasks.
* Gemini performed competitively in procedural and structured tasks.
* Prompt Chaining improved coherence, creativity, and logical consistency across all evaluated domains.

---

## Workflow

1. Load datasets using Python.
2. Select representative samples.
3. Create Single and Chained prompt versions.
4. Generate responses using Claude and Gemini.
5. Store outputs for evaluation.
6. Calculate BLEU and ROUGE metrics.
7. Perform human evaluation.
8. Compare and visualize results.

---

## Technologies Used

* Python
* Pandas
* NumPy
* NLTK
* ROUGE Score
* Hugging Face Datasets
* Google Colab
* Excel
* Large Language Models (Claude & Gemini)

---

## Repository Structure

```text
NLP-Model-Evaluation-and-Prompt-Chaining/
│
├── README.md
├── NLP_Project.ipynb
├── updated_NLP.csv
├── NLP_Final_Report.pdf
│
├── images/
│   ├── workflow.png
│   ├── bleu_score.png
│   ├── rouge_score.png
│   ├── coherence_score.png
│   ├── creativity_score.png
│   ├── logical_consistency.png
│   └── task_success_rate.png
│
└── requirements.txt
```

---

## Challenges Faced

* Manual prompt engineering and iterative prompt refinement.
* Limited API access for Claude and Gemini.
* Manual collection and logging of outputs.
* Subjectivity in qualitative evaluations.
* Variability in model responses due to prompt sensitivity.

---

## Future Improvements

* Automate prompt generation using semantic planning.
* Explore deeper multi-step prompt chains (3+ stages).
* Evaluate additional open-source LLMs.
* Extend analysis to multilingual tasks.
* Investigate multimodal prompting techniques.
* Build an interactive dashboard for result visualization.

---

## Research Report

A detailed project report is included in this repository covering:

* Literature Review
* Methodology
* Dataset Selection
* Prompt Engineering Strategy
* Experimental Setup
* Evaluation Metrics
* Results and Discussion
* Challenges and Future Work

📄 **NLP_Final_Report.pdf**

---

## Author

**Pavan Kumar Bathula**

Master's Student, Data Analytics
University of Central Florida

---

## License

This project is intended for academic, educational, and research purposes.
