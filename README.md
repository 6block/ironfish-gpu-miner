# ZK.Work_Ironfish_Miner

### AMD & Nvidia Miner for blake3_Ironfish

A git repository for ZKWorkMiner release versions

* Download releases : https://github.com/6block/ironfish-gpu-miner/releases
* Discord Group :  https://discord.com/invite/pKufwyjGFF
* Twitter : https://twitter.com/ZKWorkHQ
 
### Usage

 zkwork_ironminer [OPTIONS] --pool \<POOL\> --address \<ADDRESS\>

### Pool URL
 
 * TCP: iron.hk.zk.work:60006
 * TLS: iron.hk.zk.work:50005

### Options

 Parameter                    | Description                                               
|-----------------------------|--------------------------------------------------------------------|
| --pool <POOL>               | Specify the domain name/IP address and port of pool to connect to  |
| --address <ADDRESS>         | Specify your mining reward address                                 |
| --worker_name <WORKER_NAME> | Specify your worker name [default: "zkwork miner"]                 |
| --threads <THREADS_COUNT>   | Specify your worker thread count, deprecated [default: 48]         |  
| --batch_size <BATCH_SIZE>   | Specify batch size, deprecated [default: 573440000]                |
| --verbosity <VERBOSITY>     | Specify the verbosity [options: 0, 1, 2, 3] [default: 0]           |
| --tls                       | Connect to server over tls                                         |
| -h, --help                  | Print help                                                         |
| -V, --version               | Print version                                                      |

### ZKWorkMiner 0.1.8

_Changes_

- Added support connect to pool over tls. 
- Added support specify the verbosity.

### ZKWorkMiner 0.1.7

_Changes_

- Added support for IRON for AMD cards. 
- Fixed Illegal instruction crash on some CPU.

