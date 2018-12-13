# cilium-etcd
Scripts to install etcd operator, etcd cluster and cilium

Assuming you have the K8s cluster up and running, follow these steps to setup cilium

```
git clone https://github.com/manojbadam/cilium-etcd.git
cd cilium-etcd
kubectl apply -f etcd-operator.yaml
# generate the certs and replace the markup {{}}
# TODO: Add scripts
kubectl apply -f cilium-etcd-cm.yaml
kubectl apply -f cilium-etcd-cluster.yaml
kubectl apply -f cilium-ds.yaml
```



