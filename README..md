# Character Details Extraction Script
This repository contains a Python script to extract structured details about characters from a collection of short stories. The script processes unstructured narrative data using TF-IDF embeddings and the Mistral AI API, transforming it into a structured JSON format.

## Problem Statement
Develop a script to extract structured details about characters from stories in a provided dataset and output the required details in JSON format. The goal is to transform unstructured narrative data into a structured format using embeddings and processing techniques.

## Requirements
- Python 3.8+
- Libraries: Install required dependencies using pip: `pip install chromadb openai requests mistralai scikit-learn`

## Dataset
- The dataset consists of multiple text files hosted on a GitHub repository:[LangChain Assignment Dataset](https://github.com/deep-stack/langchain-assignment-dataset/tree/main/stories)

## Usage Instructions
### Step 1: Clone the Repository:
`git clone https://github.com/your-username/langchain-character-extraction.git
cd langchain-character-extraction`

### Step 2: Set Up Mistral API Key
Replace YOUR_API_KEY with your actual Mistral API key:
`python extract_character_details.py`

### Step 3: Run the Script
Run the script to fetch details about a character:
`python extract_character_details.py`

### Step 4: Input Character Name
Provide the character name as a query (e.g., Jon Snow).

### Step 5: View Results
The script outputs the structured details in JSON format.

### Example Output
Query: "Jon Snow"

{
"name": "Jon Snow",
"storyTitle": "A Song of Ice and Fire",
"summary": "Jon Snow is a brave and honorable leader
who serves as the Lord Commander of the Night's Watch and
later unites the Free Folk and Westeros against the
threat of the White Walkers.",
"relations": [
{ "name": "Arya Stark", "relation": "Sister" },
{ "name": "Eddard Stark", "relation": "Father" },
],
"characterType": "Protagonist"
}


