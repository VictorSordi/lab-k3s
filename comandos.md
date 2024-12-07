
curl -sfL https://get.k3s.io | sh 

Adicionar mais nós:
curl -sfL https://get.k3s.io | K3S_URL=https://myserver:6443 K3S_TOKEN=mynodetoken sh -

apt install bash-completion -y
apt install net-tools unzip -y

git clone https://github.com/ahmetb/kubectx /opt/kubectx

ln -s /opt/kubectx/kubens /usr/local/bin/kubens
ln -s /opt/kubectx/kubectx /usr/local/bin/kubectx


echo 'source <(kubectl completion bash)' >> ~/.bashrc
kubectl completion bash > /etc/bash_completion.d/kubectl
echo 'complete -F __start_kubectl k' >> ~/.bashrc

sudo vi /etc/rancher/k3s/registries.yaml

kubectl get pods -o wide
kubectl describe svc redis-server
kubectl get nodes -o wide