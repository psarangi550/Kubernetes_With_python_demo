# <ins> Kubernetes Tutorial Demo </ins> #

- **Pods In Kubernetes**

    - `pods` are the smallest unit in the `kunbernertes world`
    
    - in case of the `docker world` the `containers` were the smallest unit possible 

    - the `container` exists inside the `pods` , we can create single or multiple `container` inside the `pod`

    - all the `container` inside the `pod` share the `same volume` and `share network resources` such as `IP Address`

    - `container` present in one pod `can't be shared` with `pod` present in another `server` , one `pod` should be `present for one server which can be physical or virtual in nature`

    - when `containers` were dependent on each othwer and need to be spinned then we can spin them with in the same `pod`

    - `muiltiple container` with same `name space` can exist inside the `kubernetes pod`

    - most common usage is `one constainer per single pod`

    - each pod must be located in the same server of the kubernetes cluster

    - we can't spread the `container in the pod` accross multiple server in kubernetes cluster


- **Kubetnetes cluster and nodes**

    - `kubernetes cluster` consist of `Nodes` , where the `Nodes` are the `Server` which can be `bare minimal server/physical server` or a `virtual server`

    - there can be `multiple nodes` inside the `kuybernetes cluster` where `different node belong to the different data-center in different part of nthe world`

    - But mostly the `nodes inside the kubernetes cluster` were present very close to each other in  order to perform each `job` more efficiently

    - inside of the `nodes` there can be `multiple pods` present which is the `smallest unit of the kubernetes`

    - inside the `pods` there will be `one or more container` but mostly `one container per pod` are mostly used

    - kubernestes will create the `different pods` inside `different nodes` which is in the `kubernetes cluster`

    - our jobs is to create those `nodes` and corresponding `kubnernetes cluster based on those nodes`

    - nodes will not be created `automatically` from the cluster, once the `nodes and corresponding cluster been formed` then `kubernetes will automatically create pods on multiple nodes`

  - **How the Nodes communicate with each other and How the nodes were mmanaged inside the kubernetes cluster**

        - in a `kubernetes cluster` there will be `one master node` and `other node` called `worker nodes`
        
        - the `master node` which actually manages the `worker node` and `master node` job ios also to `distribuite the load` accross all the `worker load` so that no resources will be `over utilized or under utilized`

        - all the `pods` which container the `container application` will be shared or distributed among the `worker nodes`

        - `Master node` run the `system pod` which is responsible for `actual work of the kubernetes cluster`

        - `Master node` also have the `pods` which are the `system pod` which actually run the `kuibernetes cluster` and `worker node associated with the kubernetes cluster`

        - `Master node` inside the `kubernetes cluster` called as the `control plane` does not run the `client application` but rather run the `kubernetes cluster using the system pods`





