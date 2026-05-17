# Thesis-An-Exploratory-Case-Study-of-LLMs-for-Security-Test-Generation
This final thesis has been carried out at the School of Engineering at Jönköping University within Computer Engineering 2026.

This thesis explores test case generation by LLMs, with a focus on security test cases specifically, 
and assesses how well the generated test cases cover the security categories provided by OWASP
Top 10 for 2025. Due to AI and LLMs being increasingly common as a tool for test case generation
in software development, this thesis examines how successful different LLMs are at generating security test cases 
that satisfies the relevant OWASP security vulnerabilities, 
and to which extent human intervention might be necessary. 

# Large Language Models
The following models are used for security test case generation and have not undergone fine-tuning:

- OpenAI GPT-5.2

- Gemini 3.1 Pro

- Claude Sonnet 4.6


# Prompt for Generating Test Cases from User Stories
Execute the following prompt for each user story using a model. 

```text
Generate test cases for the following user story. Present the output as a table using the standardized test case template 
with the following fields: 
Test Case
Title/Scenario
Preconditions
Test Steps
Expected Results
Environment Specification
  
As a Software company Customer, I want the mobile client to observe the principle of "least privilege”
```
> Note: The user story above is part of the prompt and is provided as an example. Replace it with the target user story being tested when running the prompt.

# How to Reproduce Results 

1. Use the predefined user stories provided in this repository.
2. For each model, use every user story exactly once with the prompt template above to generate test cases.
