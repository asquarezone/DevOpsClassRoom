# Kubeadm Installation
1. Ensure you have more than one linux with following [flavors](https://kubernetes.io/docs/setup/independent/install-kubeadm/#before-you-begin) 
2. Ensure following ports are [open](https://kubernetes.io/docs/setup/independent/install-kubeadm/#check-required-ports)
3. Install docker runtime on  master & all nodes by following [here](https://kubernetes.io/docs/setup/cri/#docker)
4. Install kubeadm components on master & all nodes by following [here](https://kubernetes.io/docs/setup/independent/install-kubeadm/#installing-kubeadm-kubelet-and-kubectl)
5. Create the kubernetes cluster
    * Login into master, become a root user (sudo -i)
    * execute ```kubeadm init```
    * make the note of kubeadm join command 
    * now become the non root user (exit) and create kubeconfig
    * install pod network on master 
    * log in to the nodes become root user & execute kubeadm join command which you have copied
    * [Refer](https://kubernetes.io/docs/setup/independent/create-cluster-kubeadm/#instructions)