## Project 1: Automate infrastructure setup with a CloudFormation template: Deploy a Static Website on AWS S3 with CloudFormation ##

### Steps I used ###
1. Make the website: (html and css)
2. Write the _Yaml_ document to set up the bucket: to host the website, its bucket policy and its outputs.
3. Enable programmatic access by installing AWS CLI, running `aws configure` on a terminal and inputting _access key_ and _secret code_.
4. Use AWS CLI to deploy and manage resource: Use `aws cloudformation create-stack` to create the stack of resources and specify parameters, essentially for the S3 bucket.
5. Use `aws s3 sync` to copy local files to the S3 bucket
6. Access the bucket using the outputted public url




__NOTES__
- I created an IAM user having programmatic CLI access, set up Multifactor Authentication for the user and created a group having least privilege for the job added the user to it.
- I learned to troubleshoot problems programmatically while creating the stacks with `aws cloudformation describe-stacks --stackname` and on the console with _Events_ tab under _Cloudformation_ .
- I was able to update the website, just by altering the website files locally and syncing it to the bucket with `aws s3 cp`.
- I learned to troubleshoot problems with _Yaml_ files and configurations. 
