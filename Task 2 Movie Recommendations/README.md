## Content based Movie Recommendation system
A content based movie recommender system using vectorization and cosine similarity for deciding five closest movies (most similar movies) in multi-dimensional vector space.

🔗[Project is live on Streamlit](https://movie-recommendation-system-4ng5fkkpghf5hyjrgiw9ej.streamlit.app/)

```bash
├── Types of Recommendations
    ├── Content Based
    ├── Collaboration Based
    └── Hybrid
```

### Vectorization:
- In Machine Learning, vectorization is a step in feature extraction. The idea is to get some distinct features out of the text for the model to train on, by converting text to numerical vectors.
  
  ![postor](https://github.com/Bilal-Javed-Goraya/Info aid tech-Machine learning intern\Task 2 Movie Recommendation System/blob/main/photos/vectorization.gif)
  
- **Vector creation**
  
    Finally, a sparse matrix is created for the input, out of the frequency of vocabulary words. In this sparse matrix, each row is a sentence vector whose length (the columns of the matrix) is equal to the size of the vocabulary.

  ```from sklearn.feature_extraction.text import CountVectorizer```
  
  ```cv = CountVectorizer()```
  
  ```X = cv.fit_transform(sents)```
  
  ```X = X.toarray()```

### Cosine Similarities:
- Cosine similarity is used as a metric in different machine learning algorithms like the KNN for determining the distance between the neighbors.
    
- In recommendation systems, it is used to recommend movies  with the same similarities and for textual data, it is used to find the similarity of texts in the document.

![Cosine similarities](https://github.com/Bilal-Javed-Goraya/Info aid tech-Machine learning intern\Task 2 Movie Recommendation Systemblob/main/photos/cosine-similarity.jpg)

  ```from sklearn.metrics.pairwise import cosine_similarity```

  ```data_trans = cosine_similarity(data_trans)```


```bash
├── Data Features used for this project
├   ├── overview
├   ├── genres
├   └── keywords
├   └── cast
├   └── crew
```


🔗[You can download TMDB Movie Dataset from here](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?select=tmdb_5000_movies.csv)
