
# LlamaIndex with Toy Datasets (Titanic Dataset)

This project demonstrates how to use **LlamaIndex** (formerly known as GPT Index) to interact with toy datasets like the Titanic dataset from Kaggle. The goal is to generate **text-to-Pandas commands** that allow natural language queries to be converted into executable Python code for data analysis.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Future Work](#future-work)
- [License](#license)

## Overview

LlamaIndex is a powerful tool that enhances the capabilities of large language models (LLMs) by integrating them with structured data, such as datasets, to answer questions, perform analysis, and generate code. In this project, I used LlamaIndex with the **Titanic dataset** from Kaggle as a toy dataset to generate **Pandas** commands in response to natural language queries.

For example, you can ask, "How many passengers survived?" and LlamaIndex will generate the corresponding Pandas command to extract that information from the dataset.

## Features

- **Natural Language Queries:** Ask questions about the dataset in plain English.
- **Automatic Code Generation:** Get executable Pandas commands generated by LlamaIndex.
- **Dataset Exploration:** Easy and intuitive interaction with datasets like the Titanic dataset.
- **Python-Powered:** The project heavily utilizes the Python programming language and libraries like Pandas for data manipulation.

## Installation

To set up the project, clone the repository and install the dependencies:


Ensure you have access to the Titanic dataset. You can download it from [Kaggle](https://www.kaggle.com/c/titanic/data).

## Usage
Run the cells within the notebook using your own OPENAPI KEY.

Example interaction:

```bash
User: "Show me the first 10 rows of the Titanic dataset."
LlamaIndex-generated command: `df.head(10)`

User: "What is the average age of passengers?"
LlamaIndex-generated command: `df['Age'].mean()`
```

You can then copy and run these commands in your Python environment to see the output.

## How It Works

LlamaIndex (formerly GPT Index) connects large language models (LLMs) like GPT with structured data like Pandas DataFrames. Here’s a simplified flow of how LlamaIndex operates in this project:

1. **Data Loading:** The Titanic dataset (or other toy datasets) is loaded into a Pandas DataFrame.
2. **Natural Language Query:** The user inputs a natural language query, such as "How many passengers were male?"
3. **Text-to-Command Conversion:** LlamaIndex processes the query and uses the context of the dataset to generate an appropriate Pandas command.
4. **Output:** The generated Pandas command is displayed, which can be run in your Python environment for data analysis.

In short, LlamaIndex allows you to leverage the power of LLMs to translate natural language queries into Python code, making it easier to interact with datasets without needing to write the code yourself.

For more info, visit: https://docs.llamaindex.ai/en/stable/#introduction

## Future Work

- **Support for Larger Datasets:** Experiment with larger and more complex datasets beyond toy examples.
- **Query Optimization:** Enhance the model’s ability to handle more complex queries and automatically execute the generated commands.
- **Visualization Commands:** Expand the project to include automatic generation of commands for data visualization (e.g., generating Matplotlib or Seaborn plots).

