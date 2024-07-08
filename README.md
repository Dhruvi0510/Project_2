1) Create a docker file 

2) Create docker image  and push to Docker Hub 

Create image with below command:- 

docker build -t pateldhruvi7195/python-app2:latest -f "C:\Users\patel\OneDrive\Desktop\Project_2\Dockerfile.txt" .

3) Push Image to Hub :-

docker push pateldhruvi7195/python-app2:latest

4) Kubenetes Setup:-

minikube start

kubectl version --client

kubectl cluster-info

5) Kubernetes Deployment:-

kubectl apply -f deployment.yaml

kubectl apply -f service.yaml

6) Kubernetes Deployment Verification:-

kubectl get pods -o wide

kubectl get services -o wide

kubectl get nodes

7) Application testing:-

 Invoke-WebRequest -Uri "http://192.168.199.228:30002"


Challenges faced During Test of application:

The port I mentioned was incorrect in service.yaml file due to which i wasn't able to connect with network. So i made changes in node port in nodeport in service file. 
