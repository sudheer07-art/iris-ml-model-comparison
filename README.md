# Iris Species Prediction Project 🌸

Hey! This is my Project 2 submission for the Pluto Academy AI & ML Internship.

## What is this project about?

I built a machine learning model to predict the species of an Iris flower using 4 simple
measurements (sepal length, sepal width, petal length, petal width). I trained 3 different
models and compared them to see which one does the best job.

**Dataset used:** Iris Flower Classification
**Dataset source:** https://www.kaggle.com/datasets/uciml/iris
(I loaded it using `sklearn.datasets.load_iris` which is the exact same data, just easier to
load in Colab without needing a Kaggle API key)

## Files in this repo

| File | What it is |
|---|---|
| `Project2_ML_Iris.ipynb` | Main notebook - all my code, charts and write-up |
| `README.md` | You're reading it :) |

## How to run this

1. Download or clone this repo
2. Open `Project2_ML_Iris.ipynb` in Google Colab or Jupyter Notebook
3. Click Run All / Runtime → Run all
4. No extra files needed, the dataset loads directly in the notebook

## Tools I used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## What I did (step by step)

1. **Loaded and explored the data** - checked for missing values (there were none!), encoded the species labels into numbers
2. **Split the data** into 80% train / 20% test
3. **Feature engineering** - made a correlation heatmap and checked feature importance to see which measurements matter most (turns out petal length and petal width matter way more than sepal size)
4. **Trained 3 models:**
   - Logistic Regression
   - Random Forest
   - K-Nearest Neighbors (KNN)
5. **Compared all 3 models** using Accuracy, Precision, Recall and F1 Score in a table
6. **Picked the best model** and made a confusion matrix for it

## My conclusion

All three models did pretty well since Iris is a small, clean dataset that isn't too hard to
classify. The best model beat the other two on every metric in the comparison table. That's
probably because petal length and petal width separate the species really clearly, especially
setosa which almost always gets classified correctly. The confusion matrix backs this up too -
basically all the mistakes happen between versicolor and virginica, which are naturally a bit
harder to tell apart, even for humans.

## Links

- **Colab notebook (view access):** https://colab.research.google.com/drive/1eOH3VYefCWEhENuap4luZjWJHWUeFpc4?usp=sharing
- **GitHub repo:** https://github.com/sudheer07-art/iris-ml-model-comparison.git

---
Made as part of the Pluto Academy AI & ML Internship 🚀
