# devops-k8s

For this Repo I'm doing a sample app in go to contairized and deploy K8s on GKE.

Step for CI/CD

`1 - Write Dockerfile`

`2 - Docker build`

`3 - gcloud sdk`

`4 - docker push GCP`

`5 - gcloud container clusters create dev-ops-k8s --num-nodes=2`

`6 - gcloud compute instances list`

`7 - kubectl create deployment devops-web --image=gcr.io/teste-250119/devops-k8s:v1`

`8 - kubectl get pods`

`9 - kubectl expose deployment devops-web --type=LoadBalancer --port 80 --target-port 1337`

`10 - kubectl get service`

`11 - kubectl autoscale deployment devops-web --cpu-percent=50 --min=1 --max=3`

`12 - kubectl get hpa`
