# Project2clo835

# Project2clo835

# Step 1: i fork the git repo which the professor gave to us to my local machine.

# Step 2: I made a docker image by the name of project2clo835 the command was:

 docker build -t project2clo835 .

# Step 3:  I Tag my Docker image and push it to a public Docker repository the command was:

docker tag project2clo835 anurag010/project2clo835:latest


# Step 4: the next step is to make a network here i made it by the name of project2clo.


# Step 5: I created 2 files for Kubernetes Manifests:

Deployment YAML file to deploy my Docker image.

Second for:

Service YAML file using NodePort to expose my application 

# Step 6: we need to deploy the Manifests to Kubernetes for this we need to run the following command:

1. minikube start

2. minikube status

3. kubectl apply -f deployment.yaml

4. kubectl apply -f service.yaml

5. kubectl get pods.


# Step 7: need to test the app for this run the command:

minikube ip

copy the url here i got the url: 172.18.174.62:30300

with this i get the output of current location and time.



