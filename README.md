# Oneoligo Project
Edit Similarity Join implementation using DPC++ and Intel oneAPI toolkit

### Usage: 

These parameters are just an example. In general, they depend on the dataset used.

```
mkdir build

make build PARAMS="-DDEF_NUM_STR=5 -DDEF_NUM_HASH=7 -DDEF_NUM_BITS=12 -DDEF_NUM_CHAR=4 -DDEF_K_INPUT=6 -DDEF_SHIFT=6"

./onejoin --read dataset_name --device 0 --samplingrange 5000 --countfilter 1 --batch_size 10000
```


### Update constants:

```
make update PARAMS="-DDEF_NUM_STR=5 -DDEF_NUM_HASH=7 -DDEF_NUM_BITS=12 -DDEF_NUM_CHAR=4 -DDEF_K_INPUT=6 -DDEF_SHIFT=6"
```


### Simple test:

```
mkdir build
make -j
make test-join
make test-cluster
```
### Other links

[Intel article: Enable DNA Storage on Heterogeneous Architectures with oneAPI](https://software.intel.com/content/www/us/en/develop/articles/dna-storage-heterogeneous-architectures-oneapi.html) <br>
[DevMesh project](https://devmesh.intel.com/projects/oneoligo)


