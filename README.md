# Ironfish_Miner
 * TCP: iron.hk.zk.work:60006
 * TLS: iron.hk.zk.work:50005

## Mining Tutorial
**Recommend Miner**
  * SRBMiner : https://github.com/doktor83/SRBMiner-Multi/releases
  * TeamRedMiner: https://github.com/todxx/teamredminer/releases
  * RigelMiner: https://github.com/rigelminer/rigel/releases
  * lolMiner: https://github.com/Lolliedieb/lolMiner-releases/releases

**On Ubuntu**

1. Get an Ironfish wallet address on [oreos](https://github.com/6block/ironfish-gpu-miner/releases/download/v2.0.1/zkwork_ironminer.tar.gz), [ironfish-node-app](https://ironfish.network/use/node-app) etc.
2. Download Nvidia & AMD miner from **Recommend Miner**.
3. On Nvidia & AMD: `tar -zvxf <Miner_Folder>.tar.gz && cd <Miner_Folder>`.
5. Create `run_ironminer.sh`, update your Ironfish address and set worker name for mining server.
6. Start mining with `sudo chmod +x run_ironminer.sh && ./run_ironminer.sh`.
7. Check mining log.


### SRBMiner
- Windows, Linux, CPU, AMD, NVIDIA, INTEL: [v2.7.4+](https://github.com/doktor83/SRBMiner-Multi/releases)

- POOL URL
    * TCP: iron.hk.zk.work:60006
    * TLS: stratum+ssl://iron.hk.zk.work:50005

    ```shell
    export GPU_MAX_HEAP_SIZE=100
    export GPU_MAX_USE_SYNC_OBJECTS=1
    export GPU_SINGLE_ALLOC_PERCENT=100
    export GPU_MAX_ALLOC_PERCENT=100
    export GPU_MAX_SINGLE_ALLOC_PERCENT=100
    export GPU_ENABLE_LARGE_ALLOCATION=100
    export GPU_MAX_WORKGROUP_SIZE=1024
    #!/bin/sh
    reset

    ./SRBMiner-MULTI --disable-cpu --algorithm FISHHASH --pool <POOL> --wallet <ADDRESS> --worker <WORKER_NAME>
    ```


### TeamRedMiner
- Windows, Linux, AMD: [v0.10.21+](https://github.com/todxx/teamredminer/releases)

- POOL URL
    * TCP: stratum+tcp://iron.hk.zk.work:60006
    * TLS: stratum+ssl://iron.hk.zk.work:50005

    ```shell
    export GPU_MAX_ALLOC_PERCENT=100
    export GPU_SINGLE_ALLOC_PERCENT=100
    export GPU_MAX_HEAP_SIZE=100
    export GPU_USE_SYNC_OBJECTS=1
    #!/bin/sh
    reset

    ./teamredminer -a fishhash -o <POOL> -u <ADDRESS> -p <WORKER_NAME>
    ```

### RigelMiner
- Windows, Linux, NVIDIA: [v1.19.4+](https://github.com/rigelminer/rigel/releases)

- POOL URL
    * TCP: stratum+tcp://iron.hk.zk.work:60006
    * TLS: stratum+ssl://iron.hk.zk.work:50005

    ```shell
    ./rigel -a fishhash -o <POOL> -u <ADDRESS> -w <WORKER_NAME>
    ```

### lolMiner

- Windows, Linux, AMD: [v1.93+](https://github.com/Lolliedieb/lolMiner-releases/releases)

- POOL URL
    * TCP: iron.hk.zk.work:60006
    * TLS: iron.hk.zk.work:50005 (add `--tls on`)

    ```shell
    ./lolMiner --algo FISHHASH --pool <POOL> --user <ADDRESS>
    ```