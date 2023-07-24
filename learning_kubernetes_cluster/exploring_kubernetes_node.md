# <ins> Exploring the Kubernetes Node </ins> #

- Each Node inaside the `kibernetes cluster is a server` which can be `virtual server or bare metal or physical server`

- here we have created the `virtual server` , we can connect to the `virtual server` using the `ssh protocol`

- but before connecting to the `virtual server` we need to fetch the `IP Address of the node inside the kubernetes cluster`

- we can get the `ip address` of the `minikube kubernetes cluster` using the comnmand as `minikube ip`

- we can get the `ip address` of the `kind installation tool` using the command as `vctl ps` command

- we can then `ssh` into the `minikube kubernetes cluster` using the command as `ssh docker@<minikube ip>`

- `docker` is the defasult username of the `minikube kubnerntes cluister`

- `ssh` is the standard protocol for the `management of the virtual as well as bare metal and remote server`

- if we have created the `minikube kubernetes cluster with driver as docker` using the command as `minikube start --driver=docker` then `minikube provide the ssh command to go to the local minikube kubernetes cluster` using the command as `minikube ssh`

- but if we are using the something else such as `virtuialbox or hyperv` then we need to use the command as `ssh docker@<minikube ip address>`

- the `password` for the `minikube docker user` is being `tcuser` , but while using the `hyperv` driver fopr the `minikubne cluster` we can use the command as `minikube ssh`

- also while uasing the `minikube kubernetes cluster` using the `docker as the driver` we can get into the `minikube single node kubernetes cluster` using the command as `minikube ssh`

- once we logged into the `minikube kubernetes cluster by using the ssh` then we can use the command as `docker ps` which will list all the `running container inside it`

- There were buynch of `container` which ware created inside the `kuibernetes node` which can b