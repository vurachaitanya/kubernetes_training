# kubernetes_training
Training stuff
```
•	Demonized containers : run in background
•	Interactive containers: 
•	Ctl +pq –for disconnecting to a running container without killing the docker.
•	Dhclient ---for getting ip when interphase was connected in host mode. 
•	https://github.com/amitvashist7/kubernetes-project/tree/master/setup training stuff
•	download https://storage.googleapis.com/minikube/releases/latest/minikube-windows-amd64.exe or minikube for Windows and install from command line….rename minikube.exe.
•	.\minikube.exe start --- will download the image on windows.
•	https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-with-chocolatey-on-windows
Above link has Windows curl to download kubectl for windows. (curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.10.3/bin/windows/amd64/kubectl.exe)

•	Vagrant init ---with vagrant file in current locatin.
•	Vagrant status
•	Vagrant ssh kuber-master
•	Echo ‘export $KUBECONFIG=/etc/kubernetes/admin.conf’ >> ~/.bash.rc
•	Kubectl create –f <file/dir>
•	Kubectl get pods –o wide
•	Kubectl describe pod <pod name>
•	Kubectl delete pod <pod>
•	Kubectl delete service <pod>
•	Kubectl get rc
•	Kubectl edit rc hellowordo-controller
•	Kubectl scale –replicas=1 rc helloworld-controller
•	Kubectl delete rc helloworld-controller
•	Git repo got to deployment
•	Kubectl create –f helloworld.yml
•	Kubectl get deployments
•	Kubectl get pods
•	Kubectl get pods –show-labels
•	Kubectl rollout status deployments/helloworld-deployments
•	Kubectl expose deployment hellowrodl-deployment –type=NodePort
•	Kubectl get services.
•	Kubectl describe service helloworld-deployment
•	


```
