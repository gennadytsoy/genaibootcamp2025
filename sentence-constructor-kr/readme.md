# General Information
This is a conversational Korean Language Sentence Constructor (KLSC). 

The optimal person for the KLSC would be a beginner level individual (student) who is can read Korean, but still doesn't have enough vocabulary or understanding of tenses and particles to form a complete sentence.

The expected utilization would be for KLSC to assist a student to learn Korean day to day situational scenarios.

This document will attempt to document the findings from the sentence constructor testing of 4 GenAI models (ChatGPT, Gemini, Claude, and Gemini).

## Agent Flow
The following agent has the following states:
- Setup
- Input
- Output

### Input State
During the question state, the agent expects text input

### Output State
During the output state, the agent will generate and respond with:
- Translated sentence
- Vocabulary
- Sentence breakdown
- Additional vocabular fitting the setting

# AI Models Specifications
## Chat GPT
- Model: GPT-4
- Number of params: 175B
## Meta AI
- Model: Meta Llama 3.1
- Number of params: 70B

# Observations
## ChatGPT
The model performed as expected. It generated output as described in the prompt. I had to explicitly ask the model to not include polite suffix or particles as it was relatively obvious even for a beginner. The added explanation of other particles helped to better understand the structure of the sentence.


## Meta AI
The model performed poorly. The generated out was inconsistent, had poor choice of words for a conversational Korean. In addition, through one of the refinement attempts the model provided 1 vocabulary word in Russian.

## Summary
ChatGPT had a more complete response with a much better conversational Korean choice of words.
Meta AI can be improved further with additional prompt guidelines.