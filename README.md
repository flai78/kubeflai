# kubeflai
Kubernetes test

Create mssql pswd

kubectl create secret generic mssql --from-literal=password=YOUR_PASSWORD

Create the PersistentVolume:

kubectl create -f https://github.com/flai78/kubeflai/blob/master/mssql-volume-backup.yaml
https://github.com/flai78/kubeflai/blob/master/mssql-volume.yaml
View information about the PersistentVolume:

kubectl get pv mssql-volume