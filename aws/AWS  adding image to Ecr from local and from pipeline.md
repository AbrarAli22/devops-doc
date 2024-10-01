frist for local we have credientials for the ecr to push image into it

and follow commands to upload image from local
before uploading image to ecr we need to have aws cli to upload this from terminal

then in aws you have to creat a repository and named it and then assaign the desiered permissions to it and then configure this with the credientials like aws **access_key_id** and **secret** **key id**

- Retrieve an authentication token and authenticate your Docker client to your registry. Use the AWS CLI:
    
    aws ecr get-login-password --region ca-central-1 | docker login --username AWS --password-stdin 579193016008.dkr.ecr.ca-central-1.amazonaws.com
    
    Note: If you receive an error using the AWS CLI, make sure that you have the latest version of the AWS CLI and Docker installed.
    

- Build your Docker image using the following command.
    
    docker build -t laravelprod .
    

- After the build completes, tag your image so you can push the image to this repository:
    
    docker tag laravelprod:latest 579193016008.dkr.ecr.ca-central-1.amazonaws.com/laravelprod:latest
    

- Run the following command to push this image to your newly created AWS repository:
    
    docker push 579193016008.dkr.ecr.ca-central-1.amazonaws.com/laravelprod:latest

by applying this command we can push our image to ECR from local  


							**Form gilab Pipeline**


in pipline we have to install aws cli and same steps but here we did not need to configure we push from pipeline using variables we have to save variables in project variables

- apk add --no-cache curl unzip python3 py3-pip # Install curl, unzip, and Python pip

- pip3 install awscli --upgrade --user # Install AWS CLI using pip

- export PATH=$PATH:$HOME/.local/bin # Add pip installed awscli to the PATH

- aws configure set aws_access_key_id $AWS_ACCESS_KEY_ID # Configure AWS Access Key ID

- aws configure set aws_secret_access_key $AWS_SECRET_ACCESS_KEY # Configure AWS Secret Access Key

- aws configure set default.region $AWS_DEFAULT_REGION # Configure Default Region

- aws --version # Verify installation


- echo "Logging in to ECR..."

- echo $(aws ecr get-login-password --region $AWS_DEFAULT_REGION) | docker login --username AWS --password-stdin $AWS_ACCOUNT_ID.dkr.ecr.$AWS_DEFAULT_REGION.amazonaws.com

- echo "Building the Docker image..."

- docker build -t $ECR_REPOSITORY .

- echo "Tagging the image..."

- docker tag $ECR_REPOSITORY:latest $AWS_ACCOUNT_ID.dkr.ecr.$AWS_DEFAULT_REGION.amazonaws.com/$ECR_REPOSITORY:latest

- echo "Pushing the image to ECR..."

- docker push $AWS_ACCOUNT_ID.dkr.ecr.$AWS_DEFAULT_REGION.amazonaws.com/$ECR_REPOSITORY:latest

these variables are decelerize in this section and get values from project variables