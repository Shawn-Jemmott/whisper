aws configure
aws eks update-kubeconfig --region us-east-2 --name whisper-stt
aws sts get-caller-identity

kubectl version

kubectl get ep whisper  
kubectl get svc whisper
kubectl get pods
kubectl get nodes
kubectl cluster-info
kubectl logs whisper-6bc8f8c7b6-vshlq

kubectl create -f https://raw.githubusercontent.com/Shawn-Jemmott/whisper/main/stt.yaml