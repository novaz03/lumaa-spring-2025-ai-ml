# AI/Machine Learning Intern Challenge: Simple Content-Based Recommendation

---

## Overview

This model uses a **TF-IDF** algorithm and cosine similarity algorithm for content-based recommendation on a movie dataset. The raw data is obtained from *movies.csv* from https://www.kaggle.com/datasets/harshshinde8/movies-csv. (Apache 2.0 lisense). The input is a short text description, provided by the user, and the output is the list of 5 most similar movies from the dataset.

### Example Use Case

- The user inputs:  
  *"I love thrilling action movies set in space, with a comedic twist."*  
- The system outputs:
|    | original_title                 | similarity | overview                                                                                     |
|----|--------------------------------|------------|----------------------------------------------------------------------------------------------|
|3720| My Big Fat Independent Movie   | 0.183612   | This film is a spoof along the lines of 'Scary Movie' ...                                    |
|4380| Clean                          | 0.182749   | After losing her husband to a heroin overdose, ...                                           |
|3350| Jackass: The Movie            | 0.160794   | Johnny Knoxville and his crazy friends engage in various stunts ...                          |
|1040| Scary Movie 2                 | 0.133903   | While the original parodied slasher flicks like 'Scream' ...                                 |
|2390| Arn: Tempelriddaren           | 0.085616   | Arn, the son of a high-ranking Swedish nobleman, is sent to a monastery ...                  |


---

## Requirements

1. **Dataset**  
   - Use a **small** public dataset of items (e.g., a list of movies with plot summaries, or other textual descriptions).  
   - Make sure the dataset is easy to handle (maybe 100–500 rows) so the solution remains quick to implement and run.  
   - Include the dataset in your forked repository *or* provide instructions/link on how to download it.  

2. **Approach**  
   - **Content-Based**: At a minimum, use text similarity to recommend items.  
     - For instance, you can transform both the user’s text input and each item’s description into TF-IDF vectors and compute **cosine similarity**.  
   - Return the **top N** similar items (e.g., top 5).

3. **Code Organization**  
   - You may use a **Jupyter Notebook** or **Python scripts**.  
   - Keep it **readable** and **modular** (e.g., one section for loading data, one for building vectors, one for computing similarity, etc.).  
   - Briefly comment or docstring your key functions/sections.

4. **Output**  
   - When given an input description (e.g., `"I like action movies set in space"`), your system should print or return a list of recommended items (e.g., 3–5 titles).  
   - Include the similarity score or rank if you’d like.

5. **Summary & Instructions**  
   - A short `README.md` that includes:
     - **Dataset**: Where it’s from, any steps to load it.  
     - **Setup**: Python version, virtual environment instructions, and how to install dependencies (`pip install -r requirements.txt`).  
     - **Running**: How to run your code (e.g., `python recommend.py "Some user description"` or open your notebook in Jupyter).  
     - **Results**: A brief example of your system’s output for a sample query.

---

## Deliverables

1. **Fork the Public Repository**  
   - **Fork** this repo into your own GitHub account.

2. **Implement Your Solution**  
   - Load and preprocess your dataset (e.g., read CSV, handle text columns).  
   - Convert text data to vectors (e.g., TF-IDF).  
   - Implement a function to compute similarity between the user’s query and each item’s description.  
   - Return the top matches.
   - Salary expectation per month (Mandatory)

3. **Short Video Demo**  
   - In a `.md` file (e.g., `demo.md`) within your fork, paste a link to a **brief screen recording** (video link).  
   - Demonstrate:
     - How you run the recommendation code.  
     - A sample query and the results.

4. **Deadline**  
   - Submit your fork by **Sunday, Feb 23th 11:59 pm PST**.

> **Note**: This should be doable within ~3 hours. Keep it **straightforward**—you do **not** need advanced neural networks or complex pipelines. A simple TF-IDF + cosine similarity approach is sufficient.

---

## Evaluation Criteria

1. **Functionality**  
   - Does your code run without errors?  
   - When given an input query, does it successfully output relevant items?

2. **Code Quality**  
   - Clear, commented code (where it counts).  
   - Logical steps (load data → transform → recommend).

3. **Clarity**  
   - Is your `README.md` straightforward about setup, how to run, and what to expect?

4. **ML/Recommendation Understanding**  
   - Basic implementation of a content-based recommendation approach (vectorization, similarity measure).

**We look forward to seeing your solution!** Good luck!
