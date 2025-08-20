
# Test Case Generator Agent for Copilot Studio

This repository contains the prompt instructions and configuration details for a custom Copilot Studio agent designed to automatically generate high-quality software test cases based on user-provided specifications.

## 🧠 Agent Purpose

The agent acts as an expert in software testing. It analyzes functional specifications and produces structured outputs including:

- Product risks
- Equivalence partitions and boundary values
- Functional test cases (positive and negative)
- Non-functional test cases (e.g., performance, usability, accessibility)
- Impact analysis on existing functionality

## 🛠️ How It Works

Once the user provides their feature or system specifications (in one or multiple parts), the agent performs a step-by-step analysis and returns the results in a structured format using tables and Gherkin-style test steps.

## 🧾 Prompt Structure

The agent follows a strict instruction set that includes:

1. **Risk Identification**
2. **Equivalence Class Analysis**
3. **Functional Test Case Suggestions**
4. **Non-Functional Test Case Suggestions**
5. **Impact Analysis**
6. **Remarks and Observations**

The agent avoids self-introduction and directly begins with the analysis process.

## 💬 Suggested Prompts

To help users interact effectively with the agent, the following prompt suggestions can be configured in Copilot Studio:

| Prompt Title         | Prompt Message                                                   |
|----------------------|------------------------------------------------------------------|
| Generate Test Cases  | I have a feature spec. Can you generate test cases for it?       |
| Analyze Risks        | Can you identify product risks from my requirements?             |
| Edge Case Testing    | Help me create test cases for edge and boundary scenarios.       |
| Impact on Existing   | How will this new feature affect existing functionality?         |
| User Story to Tests  | Here's a user story. Can you generate test cases from it?        |
| Multi-Part Input     | My spec is large. I’ll send it in parts. Wait for all parts.     |

## ⚙️ Optional Capabilities

Depending on your use case, you may choose to enable the following features in Copilot Studio:

- **Code Interpreter (Recommended):** For dynamic test data generation, boundary calculations, and visualizations.
- **Web Search (Optional):** To reference external standards or testing guidelines.
- **Image Generator (Optional):** To visualize test flows, state transitions, or UI accessibility layouts.

## 📂 Repository Contents

- `prompt-instructions.txt` – Full prompt used to configure the agent
- `suggested-prompts.txt` – List of suggested prompt titles and messages
- `README.md` – This file

## 📌 Notes

- The agent is designed to assist, not replace, human judgment. All outputs should be reviewed critically.
- You can extend the prompt to include domain-specific testing strategies or integrate it with CI/CD pipelines.

---

Feel free to fork, adapt, and integrate this agent into your own testing workflows!
