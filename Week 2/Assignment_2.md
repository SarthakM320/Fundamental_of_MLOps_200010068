# Assignment for Week 2 

## MLOps Assignment Github repo link :
```
https://github.com/SarthakM320/MLOps_Assignment
```
## Steps used to accomplish this assignment:
```
# Making a Folder
mkdir MLOps_Assignment
cd MLOps_Assignment

# Initializing git repo
git init
git remote add origin https://github.com/SarthakM320/MLOps_Assignment
git branch -M main

# Initializing DVC
dvc init

# Then the data was downloaded and added

dvc add data/creditcard.csv
git add data/creditcard.csv.dvc data/.gitignore
git commit -m "Data added"

dvc remote add -d storage s3://mlopsassignment2/datastore
git add .dvc/config
git commit -m "Storage added"
dvc push
git push origin main


```
