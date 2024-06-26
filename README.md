# Arabic-Font-Recognition

## file structure
:small_red_triangle: make sure to create the data directory  and its sub directories like mentioned below 
becauase i depend on this route for loading and saving images after processing 

```
├──  data (will be ignored in git because it is large , but should be local in this directory as it will be used in the project)
|   ├── processed      <- The final, canonical data sets for modeling.
│           ├── font-dataset      <- The final, canonical data sets for modeling.
│                   ├── (IBM Plex Sans Arabic)
│                   ├── (Lemonada)
│                   ├── (Marhey)
│                   ├── (Scheherazade New)      
│   └── raw            <- The original, immutable data dump.
│           ├── font-dataset      <- The original, immutable data dump.
│                   ├── (IBM Plex Sans Arabic)
│                   ├── (Lemonada)
│                   ├── (Marhey)
│                   ├── (Scheherazade New)
├── models             <- Trained and serialized models, model predictions, or model summaries (pickles or  joblib files )
│
├── requirements.txt   <- The requirements file for reproducing the necessary environment (numpy , pandas,  etc,....)
├── src                <- Source code for use in this project.     
│   ├── preprocessing           <- Scripts to download / process / Augment data
│   │   
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to build and  train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
|   |---Scripts         <- contain any other scripts that are used in the project(extract certain features, plot some graph , etc ,.. ) 
│    
```