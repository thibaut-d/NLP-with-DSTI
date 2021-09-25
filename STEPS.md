# Steps taken in NLP playground with DSTI

## Git

- Create a repository with a readme and .gitignore on GitHuib
- git clone it locally with: ```git clone https://github.com/thibaut-d/NLP-with-DSTI.git```
- Create a develop branch: ```git checkout -b develop```
- Create this file on develop locally
- Save it locally
- Add it to staging area with: ```git add .```
- Commit it: ```git commit -m "my comment"``` with -m say it is for the message
- Push it: ```git push```
- Actually for the first time we need to write:  ```git push --set-upstream origin develop```
- See this directory in develop version on GitHub: <https://github.com/thibaut-d/NLP-with-DSTI/tree/develop>

## Data Acquisition

- receive data set from WeTransfer (ink thorugh Email)
- create an S3 Bucket with (public) access for everyone who needs access
    s3://dsti-ml-nlp-class/Data/
    https://dsti-ml-nlp-class.s3.eu-west-3.amazonaws.com/Data/
    e.g. for a specific file: https://dsti-ml-nlp-class.s3.eu-west-3.amazonaws.com/Data/Mr_Tochukwu_statement-part2.csv
- upload the files
