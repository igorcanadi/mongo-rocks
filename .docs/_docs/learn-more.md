---
docid: learn-more
title: Learn More
layout: docs
permalink: learn-more.html
---

### Overview

Back in 2014, MongoDB released its modular storage engine API, allowing storage engines to integrate seamlessly with MongoDB data interface. MongoRocks is one such integration, targeting RocksDB key-value store. It was originally developed and open sourced by Facebook and used by [Parse](https://parse.com).

### RocksDB

RocksDB is a key-value library based on Log Structured Merge Trees. It is maintained by the Facebook Database Engineering Team, and is based on LevelDB, by Sanjay Ghemawat and Jeff Dean at Google. If you want to learn more about RocksDB, check out [rocksdb.org](http://rocksdb.org).

### Getting started

There are two ways you can get started with MongoRocks:

* The first one is to compile the database from source. To do that, follow the instructions on our [Github page](https://github.com/mongodb-partners/mongo-rocks/blob/master/README.md).
* You can also download [Percona Server for MongoDB](https://www.percona.com/software/mongo-database/percona-server-for-mongodb), which includes MongoRocks integration and comes with support from experts at Percona.

### Running MongoRocks

Once you have MongoDB with MongoRocks installed, to select RocksDB storage engine, run:

```
$ ./mongod --storageEngine rocksdb
```

With MongoRocks up and running, you can issue the following command in Mongo shell to check RocksDB metrics:

```
db.serverStatus()["rocksdb"]
```

### Rocks-strata

Rocks-strata is a tool that lets you easily backup MongoRocks instance. Check out its [Announcement](http://blog.parse.com/learn/engineering/strata-open-source-library-for-efficient-mongodb-backups/) and [Github page](https://github.com/facebookgo/rocks-strata)

### Talks

Here's a list of talks about MongoRocks from which you can learn more:

* [MyRocks, MongoRocks and RocksDB, Percona Live 2016](https://www.youtube.com/watch?v=s_MCe1noDz0)
* [Doing More with Less with RocksDB and MongoRocks at Facebook, MongoDB Open House](https://www.youtube.com/watch?v=TViH6wFAD5w)
* [Running MongoRocks in Production, Percona Live 2016](https://www.youtube.com/watch?v=JKGKwUjyKR0)

