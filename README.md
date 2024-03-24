# Writing a Promise
This repository is an aid for the [Writing a Promise](https://kratix.io/docs/workshop/writing-a-promise)
section of the Kratix workshop.

To install:
```
kubectl apply -f promise.yaml
```

To make a resource request:
```
kubectl apply -f resource-request.yaml
```

### Run local

```shell
docker run \
  -v ${PWD}/test-input:/kratix/input \
  -v ${PWD}/test-output:/kratix/output kafka-promise:test
```