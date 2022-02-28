A container image that tests whether a container enviroment is vulnerable to escapes via CVE-2022-0492. Best to execute under a new container running an image built with:

```
$ cd can-ctr-escape-cve-2022-0492
$ docker build -t can-ctr-escape-cve-2022-0492:latest .
```

A pre-built image is available at `us-central1-docker.pkg.dev/twistlock-secresearch/public/can-ctr-escape-cve-2022-0492:latest`.

### Running in Kubernetes

```
kubectl run --restart Never --rm -it --image=us-central1-docker.pkg.dev/twistlock-secresearch/public/can-ctr-escape-cve-2022-0492:latest test-for-cve-2022-0492
```
