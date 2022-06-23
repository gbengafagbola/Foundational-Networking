## You can run either of the shell scripts (create.sh or update.sh) as:
./<file_name> argument_1 argument_2 argument_3

./creat.sh AwsVpcNetworking network.yml parameters.json


## The command above is equivalent of running the following:
aws cloudformation create-stack --stack-name AwsVpcNetworking --template-body file://network.yml    --parameters file://parameters.json  --region=us-east-1

## Troubleshoot
While running the AWS commands using either create.sh or update.sh file, if you face permission denied error, then you will have to grant the execute permission to the owner (yourself) explicitly as:

chmod +x update.sh 
chmod +x create.sh