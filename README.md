# Tasks! Claim 1 from each group:
## Train a model (tune parameters, observe performance, write down your findings/experience with your model.) Takeaways should be committed as a MODEL_takeaways.md:
- KNN (kinda done so easy) : ASSIGNEE
- Decision Tree : Adrian
- Logistic Regression : Vivian
- Random Forest : ASSIGNEE
## Misc. Tasks:
- Feature Engineering : Dale
- Make powerpoint/report : Joseph + Adrian + Vivian
- Improve model comparisons/evals : Vivian
- Clean up repo, README, etc. : ASSIGNEE


### **0. Development Setup**

Create and activate a Conda environment, then install the project dependencies:

```bash
conda create -n spotify-ml python=3.11
conda activate spotify-ml
pip install -r requirements.txt
python -m ipykernel install --user --name spotify-ml --display-name "Python (spotify-ml)"
```

In VS Code, open the notebook, select **Select Kernel** in the top-right, and choose **Python (spotify-ml)**.

### **1\. Project Title**

Spotify Genre Classification Using Machine Learning

### **2\. Group Members**

Joseph Molina (Team Leader), Dale Bittner, Adrian Pelaez, Vivian Rincon Dib, Hector Borjas

### **3\. Dataset**

We will use the [Spotify Tracks Dataset](https://www.kaggle.com/datasets/yashdev01/spotify-tracks-dataset/data) from Kaggle. Across 113,999 datapoints, it contains tracks across 125 music genres, with numerical features such as danceability, energy, loudness, acousticness, instrumentalness, tempo, and valence. These features describe musical characteristics and will serve as inputs for predicting each track's genre and respective classification.

### **4\. Initial Plan**

**The problem you are addressing:** Predict a song's genre based on its audio features and determine which classification algorithm performs best.

**Potential Stretch & Scalability:** As opposed to purely classification, we could provide each song with a composite of genres as a sum of percentages to account for songs which might be included in multiple categories

**The methods and techniques you intend to use:** We will implement and compare three supervised machine learning algorithms: K-Nearest Neighbors (KNN), Decision Tree, Logistic Regression, and Random Forest. Model performance will be evaluated using accuracy, precision, recall, and F1-score.

**Any preliminary steps you will take to begin your project:**

**General:**  
We will explore and visualize the dataset, examine genre classifications, handle missing values, encode categorical variables, and scale features where necessary. The data set already seems to be cleaned pretty well so there shouldn’t be too much work to do cleaning it. However, we plan on doing some feature selection or feature engineering to narrow down to the most impactful features. Looking at the data right now, the artist, album, and track name don't seem to be as useful as other features because you can have artists who create multiple genres or artists with a few or even one song. We will then split the data into training and testing sets, train each model, compare their results, and visualize performance differences to identify the most effective approach.

**Workflow:**  
We will determine a good and equitable split of tasks which allows us to all work on concurrent parts of the project with minimal overlap while maintaining group understanding and unified direction. A git repository will be used to collaboratively train the model. A timeline of deliverables will also be created, distributing and tracking tasks using a Gantt Chart for simultaneous tasks. 
