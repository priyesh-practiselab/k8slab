To Install Minikube:-

    brew update
    brew install minikube
    brew install kubectl

Check Installation:

    minikube version
    kubectl version --client

Start Cluster:

    minikube start --driver=docker

If you get an error like “docker driver not found”, install Docker Desktop first:

    brew install --cask docker
    open /Applications/Docker.app

Then retry the minikube start command.

Verify cluster:

    kubectl get nodes

Output:

NAME           STATUS     ROLES             AGE     VERSION

minikube       Ready      control-plane     2m      v1.30.0
