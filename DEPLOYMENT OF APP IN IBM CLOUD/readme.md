build docker image

login ibmcloud cli

set container-registry to global
ibmcloud cr region-set

docker tag local-image-name:tagname  icr.io/namespace/repo-name:tagname

docker push icr.io/namespace/repo-name:tagname

create a kubernetes cluster 

ibmcloud cs cluster-config cluster-name 

kubectl create -f deployment.yaml

kubectl create -f service.yml OR kubectl expose deployment/app-name --type=NodePort --port=5001 --name=app-name-service --target-port=5001



