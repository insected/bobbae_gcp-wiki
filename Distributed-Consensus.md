[Distributed consensus problem](https://en.wikipedia.org/wiki/Consensus_(computer_science)) requires agreement among a number of processes (or agents) for a single data value. Some of the processes may fail or be unreliable [in other ways](https://en.m.wikipedia.org/wiki/Byzantine_fault), so consensus protocols must be fault tolerant or resilient. 


## Logical Clocks

A logical clock is an idea put forward by Lamport in 1987 to solve possible problems caused by clock inconsistency between different machines in a distributed system. 

[https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675](https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675)

## State machine replication

Many distributed systems use [state machine replication](https://en.wikipedia.org/wiki/State_machine_replication) to synchronize data between copies, such as [HDFS](https://en.wikipedia.org/wiki/Apache_Hadoop#HDFS), [Chubby](https://medium.com/coinmonks/chubby-a-centralized-lock-service-for-distributed-applications-390571273052), and [Zookeeper](https://zookeeper.apache.org/).

### Paxos, ZAB and Raft

[Paxos](https://en.wikipedia.org/wiki/Paxos_(computer_science)) is a consensus protocol algorithm developed by Lamport in the 1990s. [ZAB](https://zookeeper.apache.org/doc/r3.4.13/zookeeperInternals.html) (ZooKeeper Atomic BoardCast) is a consensus protocol used in ZooKeeper. [Raft](https://raft.github.io/) is a  consensus protocol developed by developers at Stanford University in 2014. It was developed to be [easier to understand than Paxos](https://www.freecodecamp.org/news/in-search-of-an-understandable-consensus-algorithm-a-summary-4bc294c97e0d/
).

[The improved Paxos protocol](https://alibaba-cloud.medium.com/paxos-raft-epaxos-how-has-distributed-consensus-technology-evolved-73efb06aea0a) has been used in many distributed products, such as [Chubby](https://medium.com/coinmonks/chubby-a-centralized-lock-service-for-distributed-applications-390571273052), [PaxosStore](https://github.com/Tencent/paxosstore), [Alibaba Cloud X-DB](https://www.alibabacloud.com/blog/when-databases-meet-fpga-achieving-1-million-tps-with-x-db-heterogeneous-computing_594147), and [Ant Financial OceanBase](https://www.alibabacloud.com/product/oceanbase). It is generally believed that the Raft protocol has lower performance than Paxos because it only allows committing entries in sequence. However, [TiKV](https://tikv.org/) that uses Raft officially declares that it has made many optimizations on Raft and has significantly improved the performance of Raft. [POLARDB](https://www.alibabacloud.com/product/polardb) is another Alibaba Cloud database that also uses Parallel-Raft to implement the parallel commit capability in Raft. 


[Raft](https://www.hashicorp.com/resources/raft-consul-consensus-protocol-explained
) works by electing a leader in the cluster. The leader is responsible for accepting client requests and managing the replication of the log to other servers. The data flows only in one direction: from leader to other servers.



[Raft](https://www.geeksforgeeks.org/raft-consensus-algorithm/
) uses randomized election timeouts to ensure that split votes are rare and that they are resolved quickly. To prevent split votes, election timeouts are chosen randomly from a fixed interval (e.g., 150–300ms). This spreads out the servers so that in most cases only a single server will time out; it wins the election and sends heartbeats before any other servers time out. The same mechanism is used to handle split votes. Each candidate restarts its randomized election timeout at the start of an election, and it waits for that timeout to elapse before starting the next election; this reduces the likelihood of another split vote in the new election.


In Raft, the leader handles inconsistencies by forcing the followers’ logs to duplicate its own. Conflicting entries in follower logs will be overwritten with entries from the leader’s log.

### DHT, CRDT and Models for Consistency

Many real-world systems, even global financial networks, choose availability over consistency, so that people can get on with business. There are different ways to go about this. Some of them, based on [coordination protocols]( https://medium.com/@mena.meseha/understanding-of-consistency-in-distributed-systems-27da174cc05a
 ) are complicated to get right; they involve all sorts of special roles and rules.

A [distributed hash table](https://en.wikipedia.org/wiki/Distributed_hash_table) (DHT) is a distributed system that provides a lookup service similar to a hash table: key-value pairs are stored in a DHT, and any participating node can efficiently retrieve the value associated with a given key. 

A [conflict-free replicated data type](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type) (CRDT) is a data structure which can be replicated across multiple computers in a network, where the replicas can be updated independently and concurrently without coordination between the replicas, and where it is always [mathematically possible to resolve inconsistencies]( http://dist-prog-book.com/chapter/7/langs-consistency.html  ) that might come up.

CRDTs let you [avoid conflict by defining rules](https://hackmd.io/@XYOAnQcjRD-lWNVnC2p2GA/S1KpBgA0V) about how changes are applied to a single data point.



### Redis CRDT


https://redis.com/redis-enterprise/technology/active-active-geo-distribution/

### Braid

https://braid.org/

### Calvin transaction protocol

https://jepsen.io/analyses/faunadb-2.5.4

### 8 Fallacies of Distributed Systems

https://github.com/bobbae/gcp/wiki/Fallacies#8-fallacies-of-distributed-computing


