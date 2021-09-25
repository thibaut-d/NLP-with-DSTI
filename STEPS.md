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

## Data Check

- setting up a Jupyter notebook
- using boto3 to connect to S3 bucket
    AWS CLI is required for this on your machine
    https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-windows.html
- following boto3 instruction for setup 
    https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html#configuration
- defining a function that puts all objects into a list
- creating a function that puts csv or xlsx files into panda dataframes
- created a function that outputs a clean dataframe by searching for TXN DATE in the first column and takes this line as header. the function also removes Columns with nan