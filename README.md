# About rook-ceph-playground

This repository contains Helmfile configurations and Kubernetes manifests for setting up a temporary Rook Ceph cluster. It is intended for testing and validating Ceph's functionality and behavior in a non-production environment.

このリポジトリには、一時的なRook Cephクラスタを設定するためのHelmfile設定とKubernetesマニフェストが含まれています。開発用（非プロダクション）の環境でCephの機能と動作をテストおよび検証するためのものです。

# Usage

Install Rook Ceph with the following command.

```bash
helmfile apply -f ./helmfiles/rook-ceph.yaml
```

Build a Ceph cluster.

```bash
kubectl apply -f ./manifests/cluster.yaml
```

Create kuberenetes resources using manifests in the manifests directory as appropriate.
