# 🛠️ Building a Custom Database Engine – Resources & Roadmap

## 📚 Books

### 1. [Database Internals](https://www.oreilly.com/library/view/database-internals/9781492040347/) — Alex Petrov

- Focus: Storage engines, indexing, MVCC, WAL, LSM trees
- Practical and modern guide to DBMS internals

### 2. [Designing Data-Intensive Applications](https://dataintensive.net/) — Martin Kleppmann

- Focus: Data models, distributed systems, consistency, scalability
- Essential for building reliable, large-scale DBs

### 3. [Readings in Database Systems (The Red Book)](http://www.redbook.io/)

- Academic papers covering decades of DB research
- Ideal for understanding cutting-edge DB designs

---

## 📺 Courses & Tutorials

### - [CMU 15-445: Intro to Database Systems](https://15721.courses.cs.cmu.edu/spring2023/schedule.html)

- By Prof. Andy Pavlo
- Slides, recorded lectures, and projects for a full DB course

### - [Build Your Own SQLite Clone](https://github.com/cstack/db_tutorial)

- Language: C
- Walks through building a database from scratch using paging, B-trees, WAL

### - [The Internals of PostgreSQL](https://www.interdb.jp/pg/)

- Japanese/English guide to PostgreSQL source code
- Great for understanding a production-grade RDBMS

### - [LSM Tree From Scratch](https://matt-rickard.com/lsm-tree-from-scratch)

- Blog post explaining and implementing an LSM tree step by step

---

## 🧠 Papers (Theory + Implementation)

1. [Architecture of a Database System](https://dsf.berkeley.edu/papers/fntdb07-architecture.pdf) — Hellerstein et al.
   Overview of how relational databases are structured internally.

2. [The Log-Structured Merge-Tree (LSM)](https://www.cs.umb.edu/~poneil/lsmtree.pdf) — Patrick O'Neil
   The basis for modern NoSQL databases like Cassandra and RocksDB.

3. [Calvin: Distributed Transactions Without Consensus](https://cs.yale.edu/homes/thomson/publications/calvin-sigmod12.pdf)
   A deterministic approach to transaction processing.

---

## 💻 Open Source Repositories

| Name                                           | Language | Description                                                |
| ---------------------------------------------- | -------- | ---------------------------------------------------------- |
| [bitcask](https://github.com/prologic/bitcask) | Go       | Bitcask key-value store (log-structured, append-only)      |
| [tinykv](https://github.com/tikv/tinykv)       | Go       | Raft + KV engine, teaches distributed storage fundamentals |
| [sled](https://github.com/spacejam/sled)       | Rust     | Modern embedded DB with crash safety and no locks          |
| [badger](https://github.com/dgraph-io/badger)  | Go       | Fast LSM-tree KV store by Dgraph team                      |
| [bustle](https://github.com/jart/bustle)       | C        | Log-structured, high-performance embedded DB               |

---

## ⚙️ Concepts to Master

| Area               | Topics                                           |
| ------------------ | ------------------------------------------------ |
| **Storage Engine** | Pages, block size, disk I/O, memory-mapped files |
| **Indexing**       | B+ Trees, LSM Trees, Hash Indexes                |
| **Concurrency**    | MVCC, locks, read/write isolation                |
| **Transactions**   | WAL, ACID, two-phase commit                      |
| **Query Engine**   | AST parsing, query planning, execution           |
| **Persistence**    | Checkpointing, journaling, crash recovery        |
| **Replication**    | Consensus (Raft/Paxos), write quorum, sharding   |

---
