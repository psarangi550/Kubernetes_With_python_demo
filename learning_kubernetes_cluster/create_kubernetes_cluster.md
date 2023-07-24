# <ins> Creating the Minikube Kubernetes cluster </ins> #

- when we are using the command `minikube status` to see the `current status of local kubernetes cluster` then we will be seeing the below error
  
  ```
        Profile "minikube" not found. Run "minikube profile list" to view all profiles.
        To start a cluster, run: "minikube start"

  ```

- we can start the `minikube kubernetes cluster` using the option as `minikube start --driver=<VM Manager that we want to use>`

- if we are using the `windows` then we can use the `driver Virtual Machine Manager as Hyper-V` for that we need to use it as

- for that we nee to use the `Powershell in Admin Mode` and write comnmand as 

    ```
        Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All
        # using this option we can enable the Hyper-v OPTION in the microsoft

        #then we can start the minikube with the option as 
        minikube start --driver=hyperv
        # this will create the single node kubernetes cluster on the Hyper-V VM manager where the same node behave as Master and Worker Node


    ```

- here i am going to use the `hyperv` over the `windows machine` hence we need to start the `minikube` using the option as `minikube start --driver=virtualbox or minikube start --driver=hyperv MinikubeSwitch for hyperV connection`

- this will help in create the `minikube kubernetes cluster with single node` inside the `Virtualbox VM Machine`

- By default a `VM of CPU=2, Memory=4000MB Disk=20000MB` will be going to get created where the `minikube kubernetes cluster` will going to  run

- By default in the `VM of the Virtual Machine which will be having the minmikube kubnernetes cluster` we will be using the `Docker as the container runtime`

- at the end we will be getting the message as `kubectl` configured to use the `minikube kubernetes cluster running on VM manager`

- we don't have to do anything to connect from the `kubectl` to connect to the `minikube cluster` that will happen automatically once the `minikube kubernetes clsuter created inside the VM`

- when we check the status after running we can see the info such as 

  - minikube
  - type: control plane
  - host: running
  - kubelet: running
  - apiserver: running
  - kubeconfig: running 

- once that done then we can create `deployment` or `services` inside the `minikube kubernetes cluster`

- when the `minikube kubernetes cluster` being created then `kubectl` is byu default connected to it and the default container runtime for that is of `Docker`

- hence the `minikube kubernetes cluster` will not be using the local `docker installation` rather it will be using the `docker container runtime under the minikube cluster`

- 