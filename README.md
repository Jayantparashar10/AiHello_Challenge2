# AiHello_Challenge2

# AI Hello Candidate Ranking System

This project implements a candidate ranking system for matching job seekers with suitable employers.  It leverages BERT embeddings for semantic similarity matching between job descriptions and candidate profiles, combined with a rule-based system to assess how well candidates meet specific job requirements.

## Table of Contents

*   [Introduction](#introduction)
*   [Features](#features)
*   [Installation](#installation)
*   [Usage](#usage)
*   [Data Format](#data-format)
*   [Code Structure](#code-structure)
*   [Dependencies](#dependencies)
*   [Contributing](#contributing)
*   [License](#license)

## Introduction

Finding the right fit for a job is crucial for both employers and job seekers. This project aims to streamline the process by providing an intelligent ranking system.  It combines the power of natural language processing (NLP) with traditional rule-based matching to provide a comprehensive assessment of candidate suitability.  The system analyzes job descriptions and candidate profiles, considering both semantic similarity and specific requirements like salary, education, experience, and location.

## Features

*   **Semantic Similarity Matching:** Employs BERT embeddings to capture the semantic meaning of job descriptions and candidate profiles, enabling accurate matching based on skills and experience.
*   **Requirements-Based Matching:**  Assesses how well candidates fulfill specific job requirements, including salary range, education level, years of experience, and preferred location.
*   **Weighted Scoring:** Combines semantic similarity and requirements matching with a weighted average, allowing for customization of the importance of each factor.
*   **Clear Output:**  Provides a well-formatted ranking of candidates for each job posting, including individual scores for similarity and requirements matching, and a final combined score.
*   **Handles Missing Data:** Gracefully handles cases where candidates or job postings lack information for certain criteria.
*   **Scalable:** Designed to handle a large number of job postings and candidate profiles.

## Installation

1.  **Clone the repository:**

```bash
git clone [invalid URL removed]  # Replace with your repo URL
cd AI_Hello_Candidate_Ranking
````

2.  **Create a virtual environment (recommended):**

<!-- end list -->

```bash
python3 -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3.  **Install the required packages:**

<!-- end list -->

```bash
pip install -r requirements.txt
```

## Usage

1.  **Prepare your data:**  Ensure your employer and candidate data are in the correct JSON format (see [Data Format](https://www.google.com/url?sa=E&source=gmail&q=#data-format) section).  The provided `employers.json` and `candidates.json` files are examples.

2.  **Run the script:**

<!-- end list -->

```bash
python rank_candidates.py
```


## Code Structure

  * `aihello_challenge2.py`: The main script containing the logic for feature extraction, score calculation, and candidate ranking.
  * `requirements.txt`: List of required Python packages.

## Dependencies

  * `pandas`
  * `numpy`
  * `transformers` (Hugging Face)
  * `torch`
  * `scikit-learn`

## Contributing

Contributions are welcome\! Please open an issue or submit a pull request.

## License

[MIT License](https://www.google.com/url?sa=E&source=gmail&q=LICENSE)  (Or specify your preferred license)

