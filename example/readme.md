## Command

# Node
kubectl get node
kubectl describe node <nama node>

# Pod
kubectl get pod
kubectl describe pod <nama pod>
kubectl get pod -o wide (melihat lengkap detail pod)
kubectl get pods --show-labels
# Mencari Pod dengan label
kubectl get pods -l <key>
# Melihat Pod yang ada di Namespace
kubectl get pod -n <nama name space>
# Delete Pod
kubectl delete pod <nama pod>
# Delete Semua Pod di Namespace
kubectl delete pod --all --namespace <nama namespace>

# Submit config file
kubectl create -f <namafile.yml>

# Namespace
kubectl get ns


# port forward
kubectl port-forward <nama pod> portHost:portPod

# Melihat Replication Controller
kubectl get rc
# Menghapus Replication Controller
kubectl delete rc <nama rc>
kubectl delete rc <nama rc> --cascade=false

# Melihat Replication Set
kubectl get rs

# Melihat daeomonset
kubectl get daemonset