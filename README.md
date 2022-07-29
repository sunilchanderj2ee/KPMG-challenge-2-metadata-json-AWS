# Sunil Chander : KPMG-challenge-2 metadata-json-AWS

## What it does
- Query the metadata of an ec2 instance within AWS and provide a json formatted output. 
- Retrieve the value of a particular data key.

## How to install
- [Create an EC2 Linux instance on AWS](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html)
- [SSH into the instance](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html)
- Install Python 3 and git on your instance 
    - `sudo yum install python3 git`
- Clone this repository
  - `git clone https://github.com/sunilchanderj2ee/KPMG-challenge-2-metadata-json-AWS`
- Install pipenv
  - `sudo pip3 install pipenv`
- Open the repository on your instance
  - `cd KPMG-challenge-2-metadata-json-AWS`
- Install project dependancies
  - `pipenv install`


## How to run
- Open the `src` folder
  - `cd KPMG-challenge-2-metadata-json-AWS/src`
- Run whichever script you need:
  - ` pipenv run python3 get_metadata.py`
  - ` pipenv run python3 get_key.py`

## How it works
- It makes use of the http://169.254.169.254/latest/meta-data link-local address. Instance metatada is provided at this link, but only when you visit it from a running instance.
- A few simple Python scripts are used to extract the required information using the above API.
- See [AWS user guide](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-metadata.html) for more info on the instance metadata API."# KPMG-challenge-2-metadata-json-AWS" 
