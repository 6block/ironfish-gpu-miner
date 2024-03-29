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
| --verbosity <VERBOSITY>     | Specify the verbosity [options: 0, 1, 2, 3] [default: 0]           |
| --tls                       | Connect to server over tls                                         |
| -h, --help                  | Print help                                                         |
| -V, --version               | Print version                                                      |

### ZKWorkMiner 2.0.1

- Added mining with exchange address.
 
### ZKWorkMiner 2.0.0

- Improve mining efficiency：**6900xt 20G**、 **3090  20G**、 **3080 18G**、 **2080ti 17G**

### ZKWorkMiner 1.0.0

_Changes_

- Added multiple GPU cards computing power in the log.
- Increased some AMD cards computing power.

### ZKWorkMiner 0.1.12

_Changes_

- Fixed only one card is used for multiple cards on the AMD platform.

### ZKWorkMiner 0.1.11

_Changes_

- Reduced CPU usage.

### ZKWorkMiner 0.1.10

_Changes_

- Added support check mining address.

### ZKWorkMiner 0.1.9

_Changes_

- Fixed the problem of incompatibility of cpu instruction set. 
- Added support for IRON for more AMD cards.

### ZKWorkMiner 0.1.8

_Changes_

- Added support connect to pool over tls. 
- Added support specify the verbosity.

### ZKWorkMiner 0.1.7

_Changes_

- Added support for IRON for AMD cards. 
- Fixed Illegal instruction crash on some CPU.

