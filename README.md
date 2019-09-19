## Build s2i image

```
docker build -t shapeblock/node:12 .
docker push shapeblock/node:12
```

## Build nginx image

```
docker build -t shapeblock/nginx-node:1.17 .
docker push shapeblock/nginx-node:1.17
```

## Import into OpenShift

```
oc import-image shapeblock/node:12 --confirm -n openshift
oc import-image shapeblock/nginx-node:1.17 --confirm
```
