Create docker image  and push to Docker Hub 
Create image with below command
docker build -t pateldhruvi7195/python-app2:latest -f "C:\Users\patel\OneDrive\Desktop\Project_2\Dockerfile.txt" .

Push Image to Hub 
docker push pateldhruvi7195/python-app2:latest

Kubenetes Setup
minikube start
kubectl version --client
kubectl cluster-info

Kubernetes Deployment
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

Kubernetes Deployment Verification
kubectl get pods -o wide
kubectl get services -o wide
kubectl get nodes

Application testing
 Invoke-WebRequest -Uri "http://192.168.199.228:30002"

 