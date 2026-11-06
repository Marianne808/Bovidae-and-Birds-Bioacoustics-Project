# Perch repository
PERCH2.0 (https://github.com/google-research/perch)

Notebooks Needed
- embed_audio
- agile_modeling
- analysis

## Work flow
- Collected over 100 confusion sound samples 
- Saved into my Training data folder under a new class name
### install jupyternotebook hub to terminal
- pip install jupyter
- command line type jupyter notebook
- run everything from terminal / desktop
### In the embed_audio notebook
- After uploading the target class and site files to volume
- Change path to match location of files
- Run entire embeddings notebook (Usually takes hours on CPU)
### In the agile_modeling notebook
- Created a new model folder in volume and changed “custom classifier path” to that folder name
- Run blocks till “search embeddings”
- Skip down to “Active Learning for a Target Class” Block and run blocks until “Train small model over embeddings”
- In “Run model on target unlabeled data” change target_class = ‘ ‘ to new class name
### In the analysis notebook 
- Change “configuration” block and “custom classifier path” to new model folder name 
#### Check by looking 
- Below “Load Existing Project State and Models” should show the list of all the models with classes including your new class name
### To load in the samples for precision modeling
-  Run until “evaluate best samples”
-  Input target class and site location
-  Run "Display Samples" block
-  Change buttons by editing "labels" code, must include target species
-  Make sure to save your results and categories in respective folders
