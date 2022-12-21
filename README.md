# kubectx

## Pre-Requisites

```bash
kubernetes cluster
```

## kubernetes cluster - minikube
[minikube setup](https://github.com/Naresh240/kubernetes/blob/main/minikube-setup/README.md)

## Install kubectx

```bash
echo "**** Install kubectx *****"

export VERSION_KUBECTX=v0.9.4
curl -LO https://github.com/ahmetb/kubectx/releases/download/${VERSION_KUBECTX}/kubectx_${VERSION_KUBECTX}_linux_x86_64.tar.gz
tar -xzvf kubectx_${VERSION_KUBECTX}_linux_x86_64.tar.gz
chmod +x ./kubectx
mv ./kubectx /usr/bin
```

## switch to another cluster that's in kubeconfig

```bash
kubectx minikube
```
![image](https://user-images.githubusercontent.com/58024415/208839777-c1f922bb-e45c-43a5-85f5-2b33d925c7cc.png)

## switch back to previous cluster

```bash
kubectx -
```

## create an alias for the context

```bash
kubectx <alias-name>=<context-name>
```
