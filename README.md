# LLM Security Evaluation and Prompt Injection Testing Framework

This project implements a simple framework to evaluate potential security vulnerabilities in Large Language Models (LLMs) using adversarial prompts. The goal is to analyze how language models respond to potentially malicious or manipulative inputs.

## Objective

The project tests LLM responses against prompts designed to simulate common security threats such as:

- Prompt Injection
- Jailbreak Attempts
- Data Leakage
- Instruction Manipulation

The framework collects model responses and flags outputs that may indicate unsafe or vulnerable behavior.

## Methodology

1. A dataset of adversarial prompts is created and stored in `prompts.csv`.
2. Prompts are passed to a language model using the HuggingFace Transformers library.
3. Model responses are collected automatically.
4. A simple rule-based analysis detects potentially insecure outputs.
5. A security report is generated summarizing the results.


## Technologies Used

- Python
- HuggingFace Transformers
- PyTorch
- Pandas

## Output

The framework generates a **security report** identifying prompts that may cause unsafe responses from the language model.

Example output fields:

- Prompt
- Model Response
- Security Flag (Safe / Potential Leak)

## Use Case

This project demonstrates a basic approach for studying **LLM behavior, robustness, and security risks**, which is an important topic in modern AI safety research.

## Future Improvements

- Add more adversarial prompts
- Implement advanced vulnerability detection methods
- Evaluate multiple LLM architectures
- Visualize security risk metrics
