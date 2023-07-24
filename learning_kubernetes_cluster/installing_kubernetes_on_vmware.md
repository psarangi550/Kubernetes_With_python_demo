# <ins> How to Run Kubernetes Cluster using VMWare VM Manager and Kind for  Creating Cluster with Docker Runtime </ins> #

- After successful installation of VMware Workstation player/pro, you will find the executables from `C:\Program Files(x86)\VMware\VMware Player` for `VMware workstation 16 player` and `C:\Program Files (x86)\VMware\VMware Workstation\` for `VMware workstation 16 pro`. Note that the Vmware workstation has three executable which include:

- **Containerd.exe**:-
  -  It is the runtime `containerd daemon` that `requires to be started` before running `any container`. 
  -  It is started on command prompt or PowerShell on windows using the `vctl system start` command

- **Containerd-shim-crx-v2.exe**:-
  - it acts as an `adapter` between the `containerd daemon` and the `container in CRX VM`.
  - It has the role of launching a `new containerd-shim-crx-v2` `process` when a `new container` is started

