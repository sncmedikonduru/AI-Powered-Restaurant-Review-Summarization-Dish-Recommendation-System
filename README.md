# Restaurant Reviews Summarization and Dish Recommendation

## Problem Statement

In this project, we aim to build a **Restaurant Reviews Summarization and Dish Recommendation System**. The system processes a dataset of restaurant reviews and automatically summarizes them, while ensuring that key information such as **restaurant names** and **recommended dishes** is preserved in the final output.

### Goals:
1. **Summarization**: Summarize customer reviews for restaurants, condensing the key information into a coherent summary.
2. **Extraction**: Ensure that important information like restaurant names and dish names are extracted and included in the summary.
3. **Recommendations**: Provide dish recommendations based on reviews.

## Project Workflow

### 1. Data Extraction
- Extract **restaurant names** from the dataset (assumed to be available in a column called `name`).
- Extract **recommended dishes** from a column such as `recommended_dishes`.

### 2. Text Generation
- Use **GPT-Neo** to generate a summary of restaurant reviews.

### 3. Summarization
- Use **BART** to summarize the generated text and condense key insights from reviews.

### 4. Post-Processing
- Ensure that the **restaurant names** and **recommended dishes** are preserved in the final summary.

## Dataset

The dataset should contain at least the following columns:
- **name**: The name of the restaurant.
- **cleaned_review**: The cleaned reviews of the restaurant.
- **recommended_dishes**: The dishes recommended by customers (optional, can be extracted from reviews if not available directly).

## Key Components

### Summarization and Text Generation
- **GPT-Neo**: Used for generating raw text summaries based on restaurant reviews.
- **BART**: Used for condensing and summarizing generated text.

### Entity Extraction
- **Restaurant Names**: Extracted directly from the dataset.
- **Dish Names**: Extracted from the dataset or inferred from reviews.

### Grammar and Refinement
- (Optional) Use **LanguageTool** for grammar correction to produce more polished summaries.
