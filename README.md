This repo is updated with new version of template support for geth 1.10

- Issue: 
    - Miners node don't automatically connect to the bootnode
        - how to fix: 
                - using admin.addPeer("enode://...@cluster_ip_miner_or_bootnode:30303") 
                - get cluster ip and put it to environment variable and update to gethconfig.toml
# Ethererum Proof of Authority Clique Kubernetes template
Use this template to start Proof of Authority network on your kubernetes cluster or locally on minikube.

## Kubernetes 
To start network using kubectl use:
sh start.sh

To start it locally in minikube use:
sh start_in_minikube.sh

To sync locally use:
sync_locally.sh (just change enode to your endpoint)

Medium article to help you get started: https://medium.com/@edi.sinovcic/ethererum-poa-clique-on-kubernetes-6e86fed0c310
