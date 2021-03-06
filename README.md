# didactic-sniffle
Repository containing data analysis of Spotify API database. The goal of the repository is to analyse the content of the data and find:
- Confirm "loudnes war" phenomenon;
- Relation between song modality and popularity;
- Relation between energy and loudness.

## 1) Dataset
The dataset was downloaded from kaggle.com (https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks) and contains music from 1921 to 2020. 

### Structure:

  ### Primary:
    - id (Id of track generated by Spotify)
    
  ### Numerical:
    - acousticness (Ranges from 0 to 1)
    - danceability (Ranges from 0 to 1)
    - energy (Ranges from 0 to 1)
    - duration_ms (Integer typically ranging from 200k to 300k)
    - instrumentalness (Ranges from 0 to 1)
    - valence (Ranges from 0 to 1)
    - popularity (Ranges from 0 to 100)
    - tempo (Float typically ranging from 50 to 150)
    - liveness (Ranges from 0 to 1)
    - loudness (Float typically ranging from -60 to 0)
    - speechiness (Ranges from 0 to 1)
    - year (Ranges from 1921 to 2020)
    
  ### Dummy:
    - mode (0 = Minor, 1 = Major)
    - explicit (0 = No explicit content, 1 = Explicit content)
    
  ### Categorical:
    - key (All keys on octave encoded as values ranging from 0 to 11, starting on C as 0, C# as 1 and so on…)
    - artists (List of artists mentioned)
    - release_date (Date of release mostly in yyyy-mm-dd format, however precision of date may vary)
    - name (Name of the song)

## 2) Tools
Main programming language used in this project is Python with elements of Pandas, NumPy and iPyhon libraries.
