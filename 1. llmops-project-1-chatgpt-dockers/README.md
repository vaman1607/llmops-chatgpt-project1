


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
kubectl create secret generic openai-secret --from-literal=API_KEY=<your api-key>
```