NEO private network with initial 100m NEO and lots of GAS (https://hub.docker.com/r/metachris/neo-privnet-with-gas/)
```
docker pull metachris/neo-privnet-with-gas
```

Start container
```
docker run -d --name neo-privnet-with-gas -p 20333-20336:20333-20336/tcp -p 30333-30336:30333-30336/tcp metachris/neo-privnet-with-gas
```

Make sure to delete any old private-net chain: 
```
rm -rf Chains/privnet
```

Use prompt on privnet
```
python prompt.py -p
```

Import wallet to get the 100m NEO
```
import wif KxDgvEKzgSBPPfuVfw67oPQBSjidEiqTHURKSDL1R7yGaGYAeYnr
```
