


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