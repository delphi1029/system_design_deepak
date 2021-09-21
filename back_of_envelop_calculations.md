# Back Of Envelop Calculations - 

### 1 billion = thousand millions (1000 millions) 
    - number of zeros in 1 billion is 9
### 1 million = thousand thousands (1000 thousands)
    - number of zeros in 1 million is 6

### 1 TB = 1000 GB
### 1 GB = 1000 MB
    - 1 GB = 10^9 bytes = 10^6 KB = 10^3 MB
### 1 MB = 1000 KB
### 1 KB = 1000 Byte
### 1 byte = 8 bit

### 1 hr = 3600 seconds
### 1 day = 1440 minutes
### 1 day = 86400 seconds

### x Million users * y KB = xy GB
### x Million users * y MB = xy TB

## Storage required for character
### ASCII (1 byte per character)
### Unicode
   - UTF-8 (variable: 1, 2, 3, or 4 bytes per character)
   - UTF-16 (variable: 2 or 4 bytes per character)
   - UTF-32 (4 bytes per character)
### Short: 2B (16 bits)
### Int: 4B (32 bits)
### Long: 8B (64 bits)
### UUID/GUID: 16B

### File: 100 KB
### Web Page: 100 KB (not including images)
### Picture: 200 KB
### Short Posted Video: 2MB
### Steaming Video: 50MB per minute
### Long/Lat: 8B

### Maximum URL Size: ~2000 (depends on browser)
### ASCII charset: 128
### Unicode charset: 143,859


## Per Period Numbers
The following numbers are heavily rounded and help determine how often something needs to happen over a period of time. For example, if a server has a million requests per day, it will need to handle 12 requests per second.


| Month         | 1 Billion     |  1 Million  | 1 Thousand |
| ------------- |:-------------:|:-----------:|:----------:|
| Day           | 32 M          |   32 K      |   32       |
| Hour          | 1.3 M         |   1.3K      |   1.3      |
| Minute        | 22 K          |   22        |   0.02     |
| Second        | 400           |   0.4       |   0.0004   |


| Day           | 1 Billion     |  1 Million  | 1 Thousand |
| ------------- |:-------------:|:-----------:|:----------:|
| Hour          |   42 M        |   42 K      |   42       |
| Minute        |   700 K       |   700       |   0.7      |
| Second        |   12 K        |   12        |   0.01     |


### More complex example:
 - 100M photos (200KB) are uploaded daily to a server.
 - 100 (number of millions) * 12 (the number per second for 1M) = 1200 uploads a second.
 - 1200 (uploads) * 200KB (size of photo) = 240MB per second.

The web servers will need to handle a network bandwidth of 240MB per second. You will therefore need a machine with high network performance to handle this bandwidth. In AWS this would translate to at least a m4.4xlarge, but it would be better to have multiple smaller servers to handle fault tolerance.

### Users
 - Facebook: 2.27B | YouTube: 2B | Instagram: 1B
 - Pinterest: 332M | Twitter: 330M | Onedrive: 250M
 - TikTok: 3.7M

### Visits
 - Facebook: 26.12B | Twitter: 6.34B | Pinterest: 1.32B
 - Spotify: 293M | Ikea: 233M | Nike: 110M
 - Argos: 54M | John Lewis: 37M |Superdry: 3.5M
 - Virgin Money: 1.8M | Aviva: 1.61M

### Cost of Operations
 - Read sequentially from HDD: 30 MB/s
 - Read sequentially from SSD: 1 GB/s
 - Read sequentially from memory: 4 GB/s
 - Read sequentially from 1Gbps Ethernet: 100MB/s
 - Cross continental network: 6–7 world-wide round trips per second.
 
### SQL Databases
 - Storage: 60TB
 - Connections: 30K
 - Requests: 25K per second

### Cache [Redis — Requests][Redis — connections]
 - Storage: 300 GB
 - Connections: 10k
 - Requests: 100k per second
 
### Web Servers
 - Requests: 5–10k requests per second

### Queues/Streams
 - [Pub/Sub — limits][Kinesis — limits][SQS — limits]
 - Requests: 1000–3000 requests/s
 - Throughput: 1MB-50MB/s (Write) / 2MB-100MB/s (Read)
