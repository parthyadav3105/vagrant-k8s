# Vagrant k8s
*Single node kubernetes cluster on vagrant vm using kubespray.*

[Kind](https://kind.sigs.k8s.io/docs/user/quick-start/) is always first choice for dev k8s cluster, it's fast!

But sometime specific workloads just refuse to run in a docker inside docker environment, this is when we need a k8s in a VM. Use this repo to create single node dev k8s cluster using kubespray inside vagrant vm.

> Note: `minikube --vm` didn't worked well for one of my workload, hence kubespray in a vm.

<hr>

### Usage:
***prerequisite:** make sure vagrant with libvirt is installed.*

Step 1: Edit `config.yaml`, if required.

Step 2: Run `vagrant up`

*Post-install you will have to setup your network plugin as you would do with kubeadm.*
<hr>



> Note: This repo is modified version of fork from [m18unet/kubespray-single-node](https://github.com/m18unet/kubespray-single-node).
>
> Note: Official kubespray repo also has a [vagrant file](https://github.com/kubernetes-sigs/kubespray/blob/master/Vagrantfile).
