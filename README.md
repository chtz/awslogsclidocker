# A simple docker wrapper for awslogs

## Pre-Conditions

AWS credentials configured:
- ~/.aws/config
- ~/.aws/credentials

## Installation (e.g. ~/.bashrc)

	alias awslogs='docker run -v ~/.aws:/root/.aws --rm -i chtzdc/awslogs:latest'

## Sample: List CloudWatch log groups

	awslogs groups

## Sample: Watch a CloudWatch log group (e.g. mygroup)

	awslogs get mygroup --watch

