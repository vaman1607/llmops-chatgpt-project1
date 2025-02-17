


# Help on FASTAPI

```
pip install "fastapi[all]"

uvicorn main:app --reload
```

# Docker Image

```
docker build -t chatgpt-project1 .

# To run docker container
docker run -d -p 8080:80 chatgpt-project1

# To push into Dockerhub registry
docker tag chatgpt-project1 yourusername/chatgpt-project1
docker push yourusername/chatgpt-project1
```

# Kubernetes code

```
# Create a kubernetes secret to store api_key
kubectl create secret generic openai-secret --from-literal=API_KEY=<your api-key>

# Create a new image as api_key is removed from code and stored as  a secret

docker build -t vaman1607/chatgpt-project:v1 .

# Push to Docker hub repository
docker push vaman1607/chatgpt-project:v1

# Deployment to local Kubernetes cluster
kubectl apply -f deploy.yaml

# Command to check the pods running
kubectl get po

# Command to check secrets
kubectl get secrets
```

## application runs on localhost:30002

# Important command for Docker macos

```
docker buildx build --platform=linux/amd64 -t vaman1607/chatgpt-project:v3 .
docker push vaman1607/chatgpt-project:v3
```

# Github actions
```

Store the below secrets under Settings> Secrets and Variables >Actions >New Repository Secret
GKE_PROJECT : "Your Google Cloud Project Name"

GKE_SA_KEY : "Key generated from Service account(Secret Key)

OPENAI_API : "Api Key to be stored".
```
