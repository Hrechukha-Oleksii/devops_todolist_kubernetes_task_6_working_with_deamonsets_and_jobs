1. How to deploy `daemonset.yml` and `cronjob.yml` to the cluster.

    - Run the daemonset from `daemonset.yml` manifest:

        cd .\.infrastructure\ && kubectl apply -f daemonset.yml
    
    - Run the cronjob from `cronjob.yml` manifest:

        cd .\.infrastructure\ && kubectl apply -f cronjob.yml


2. How to validate the solution.

    - Check logs for the `daemonset`:

        kubectl get pods && kubectl logs <"daemonset's pod name">

    - Check logs for the `cronjob`:

        kubectl get pods && kubectl logs <"cronjob's pod name">


