## Kubernetes Setup for CSW-PROD

### Pre-requisite

- Docker

- VirtualBox

- Minikube (brew install minikube) : This is required to create kubernetes cluster locally.

### How to Run

- Execute `up.sh` script from shell

    This will start following:
    - Cluster Seed on Port 3552
    - Admin Http Server on Port 7878
    - Cluster Management on Port 7879
    - Config Server on Port 4000

- Run `minikube dashboard` cmd from shell to view kubernetes dashboard where you can see logs from all the applications.

- Run `minikube service config --url` cmd from shell, which will give Config server url which can be accessible from host machine

### Shutdown Cluster

- Execute `down.sh` script from shell, which will remove all the deployments, services and statefulsets

- Run `minikube stop` to stop minikube cluster