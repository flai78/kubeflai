# kubeflai
Kubernetes test

Create mssql pswd

kubectl create secret generic mssql --from-literal=password=YOUR_PASSWORD


Create directory
mkdir /mnt/data/mssql
mkdir /mnt/data/bkp

Create the PersistentVolume:


kubectl create -f https://raw.githubusercontent.com/flai78/kubeflai/master/mssql-volumes.yaml


View information about the PersistentVolume:

kubectl get pv mssql-volume

Create MS SQL Service
kubectl create -f https://raw.githubusercontent.com/flai78/kubeflai/master/mssql.yaml