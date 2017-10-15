## Kubernetes Setup for CSW-PROD

### Pre-requisite

- Docker

- VirtualBox

- Minikube (brew install minikube) : This is required to create kubernetes cluster locally.

### How to Run

- Execute up.sh script from shell

    This will start following:
    - Cluster Seed on Port 3552
    - Admin Http Server on Port 7878
    - Cluster Management on Port 7879
    - Config Server on Port 4000

- Run minikube dashboard to view kubernetes dashboard where you can see logs from all the applications.

- Run minikube service config --url, which will give Config server url which can be accessible from host machine