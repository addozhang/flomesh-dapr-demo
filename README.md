
### Build App Image

```shell
cd nodeapp
docker buildx build -t addozhang/dapr-nodeapp --no-cache --platform linux/amd64,linux/arm64 --push .
```

### Usage of flomesh.sh

**Requires**

- [Docker](https://docs.docker.com/get-docker/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/)

Other pre-requisite utilities like `k3d`, `helm`, `jq`, `pv` if missing, will be installed via os package manager. To run the demo

- `flomesh.sh` - without any arguments, it will create and setup 4 demo `k3d` clusters, and run demo
- `flomesh.sh -h` - display usage information
- `flomesh.sh -i` - create and setup 4 demo `k3d` clusters
- `flomesh.sh -d` - run the demo
- `flomesh.sh -r` - reset the demo and deletes demo kubernetes resources
- `flomesh.sh -u` - tear down clusters
