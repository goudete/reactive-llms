# ReAct pattern for LLMs

## Context
A popular nightmare scenario for AI is giving it access to tools, 
so it can make API calls and execute its own code and generally 
break free of the constraints of its initial environment.

Let's do that now!

It's a pattern where you implement additional actions that an 
LLM can take - searching Wikipedia or running calculations for 
example - and then teach it how to request that those actions are 
run, then feed their results back into the LLM.

ReAct looks innocuous but here’s the deal: instead of asking GPT to simply do smart-autocomplete on your text, you prompt it to respond in a thought/act/observation loop. So you ask GPT to respond like:

Thought: Let’s think step by step. I need to find out X and then do Y.

Act: Search Wikipedia for X

Observation: From the Wikipedia page I have learnt that …

Thought: So the answer is …

And it is allowed to repeat as many times as necessarily, iterating towards its goal.


## 📡 Librarires 📡

```
OpenAI Python Library
https://github.com/openai/openai-python
```

## 📜 Papers / References 📜
```
The surprising ease and effectiveness of AI in a loop
https://interconnected.org/home/2023/03/16/singularity

A simple Python implementation of the ReAct pattern for LLMs
https://til.simonwillison.net/llms/python-react-pattern

```
