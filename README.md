# simple-kubernetes-cluster
Simples cluster Kubernetes utilizando Kind

Comando para criar o cluster:

kind create cluster --config config.yaml --name cluster-demo --kubeconfig config

Comando para excluir o cluster:

kind delete cluster --name cluster-demo

Criando um novo pod:

kubectl apply -f pod.yaml

Por padrão, um recurso é criado na namespace default.

Listando todas as namespaces:

kubectl get ns 

Criando uma namespace:

kubectl create ns nome-da-ns

Definindo uma namespace como padrão:

k config set-context --current --namespace default
