# AI/Machine Learning Intern Challenge: Simple Content-Based Recommendation

---

## Overview

This model uses a **TF-IDF** algorithm and cosine similarity algorithm for content-based recommendation on a movie dataset. The raw data is obtained from *movies.csv* from https://www.kaggle.com/datasets/harshshinde8/movies-csv. (Apache 2.0 lisense). The input is a short text description, provided by the user, and the output is the list of 5 most similar movies from the dataset.

### Example Use Case

- The user inputs:  
  *"A movie about life, love, and death."*  

- The system outputs:
---

|      | original_title                | similarity | overview                                                                                                           |
|-----:|:------------------------------|-----------:|:-------------------------------------------------------------------------------------------------------------------|
| 1440 | **The Fountain**             | 0.232185   | Spanning over one thousand years, and three parallel stories, The Fountain is a story...                           |
| 3720 | **My Big Fat Independent Movie** | 0.221189   | This film is a spoof along the lines of 'Scary Movie'...                                                           |
| 3350 | **Jackass: The Movie**       | 0.211145   | Johnny Knoxville and his crazy friends appear...                                                                   |
| 3190 | **Veer-Zaara**               | 0.195037   | The story of the love between Veer Pratap Singh...                                                                 |
| 2680 | **Lars and the Real Girl**   | 0.188559   | Sometimes you find love where you'd least expect it...                                                             |


---

## Notes
The Jupyter Notebook ```Data.ipynb``` is the main body of the algorithm.
1. **Dataset**  
   - Built-in code blocks for retrieving and processing the data are provided in the Jupyter Notebook.
   - A pre-processed csv file is also provided as ```'/Data/my_data.csv'```

2. **Setup**  
   - **Python**: The python version is Python 3.11.11. Run ```python3.11.11 -m venv env``` to create a virtual environment in a folder named ```'env'```
      - On Windows, run ```env\Scripts\activate``` to initiate the virtual environment.
      - On MacOS/Linux, run ``` source env/bin/activate``` to initiate the virtual environment.
   - You may run ```pip install -r requirements.txt``` to install the relevant packages. 
      - Alternatively, run ```!pip install -r requirements.txt``` in the first cell of the Jupyter Notebook.
   - **Jupyter Notebook**: Use ```pip install notebook``` to install the jupyter notebook.
      - Run ```jupyter notebook``` to launch the jupyter notebook

## Link to video:
### https://youtu.be/7a1NmnQafJY

