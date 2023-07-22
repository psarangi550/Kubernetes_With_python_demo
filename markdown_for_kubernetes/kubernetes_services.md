# <ins> Kubernetes Services In depth </ins> #

- **Which Services are running on different node inside the kubernetes cluster**
  
    - There are multiple different services running on kubernetes cluster based on the `node` whether the `Master node` or `Worker Node`

    - Those Services can be of below for `Master or Worker Node` inside the `kubernetes cluster`
      
        - `kubelet Service`
        - `kube-proxy service`
        - `container runtime service`  

    - `container runtime service` such as `docker or CRI-O or containerd` services run the `container` inside a `node or server which can be a bare metal server or virtual server`

    - `kubelet` services inside each `worker node` communicate with the `API Server Service` of the `Master Node`

    - `API Server` Service is the `main point of communication between the different node inside the kubernetes cluster`

    - `kube-proxy` Service is responsible for `main point of Network communication` between
      
      - inside of each node
      - node to node communication inside the kubernetes cluster

    - There are few other `services` present only in the `Master Node` such as 
      
      - `API Server Service`
      - `Scheduler Service`
      - `Kuber controller Manager`
      - `Cloud controller Manager`
      - `etcd services`
      - `DNS Service`
    
    - `API Server` Service is the `main point of communication between the different node inside the kubernetes cluster`

    - `Scheduler Service` is responsible for `Planning and Distributing the load between the nodes in the kubernetes cluster`

    - `Kube Control Manager` which is the `single point` which handle everything `inside the kubernetes cluster` and it also contol what happens `each node of the cluster`

    - `Cloud controller Manager` which is responsible to interact with the `cloud service provider` where the `kubernetes cluster` been running 

    - we can `rent the kubernetes cluter` from one of the `cloud provider` which can `create the nodes automatically and handle communication between the nodes `

    - if we want to deploy the `containerized application` inside the `kubernetes cluster` and make it `open` for the `outside world` and allow connection from the `outside world` then we can use the `load balancer ip address` as well , those `load balancer ip address` been provided by the `cloud service provider `

    - the `etcd` service on the `Master Node` store all the logs belong to the `operation of kubernetes cluster` and which will store the logs as `key/value pair`

    - the `DNS sercvice` on the `Master node` will help in `name resolution into the ip address` based on the `dns server mapping` for the `all the nodes in the cluster`

    - By using the `DNS Service` we can `connect two specific deployment based on the name of the deployment service` which will help in `communication between 2 different deployment service`

- **Linked Images**
![Kubernetes Deno](WhatsApp%20Image%202023-07-22%20at%209.34.32%20PM.jpeg)
