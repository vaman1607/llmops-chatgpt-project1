# llmops-chatgpt-project1
This is a simple project that demonstrates deployment to local and GKE using Kubernetes.

**Stage 1(Create application):**
- Generate an api_key from platform.openai.com
- Create an assistant_id using openai library in python
- Use the assitant_id to create threads, messages and runs for the application to interact with Chatgpt.
- Demonstrate to create Docker Image using a Docker file

**Stage 2(Kubernetes Local Cluster demonstration):**
- From Stage1 Install Kubernetes in the local.
- Create deploy.yaml file to enable deployment of the application on local Kubernetes cluster

**Stage 3(GKE demonstration):**
- Create a google cloud account
- Configure google cloud cli
- Create Kubernetes Cluster on GKE
- Deploy application on Kubernetes Cluster created.

**Stage 4(CI/CD demonstration using Github actions):**
- Create actions.yaml file for Github actions
- Create kustomization.yaml file to enable automatic updation of Docker image tag in deploy.yaml with every new update
- Demonstrate secrets used in Github to store secret keys.
- Setup actions to ensure deployment.


