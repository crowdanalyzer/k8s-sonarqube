# k8s-sonarqube
SonarQube for Kubernetes.

## Installation instructions

* Create secret for Postgres database

```sh
kubectl create secret generic postgres-pwd --from-literal=password=CodeRise_Pass
```

* Run manifests

```sh
kubectl create -f sonar-postgres.yaml
kubectl create -f sonarqube.yaml
```

* Enjoy