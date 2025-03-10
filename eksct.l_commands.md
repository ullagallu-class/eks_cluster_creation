eksctl version
eksctl create cluster -f eks-cluster.yaml
aws eks --region us-east-1 describe-cluster --name eks-cluster --query "cluster.status"
kubectl get nodes
eksctl delete cluster --name eks-cluster --region us-east-1