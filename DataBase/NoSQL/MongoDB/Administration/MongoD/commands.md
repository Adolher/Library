<sup>[MongoDB Docs MongoD Commands](https://www.mongodb.com/docs/manual/reference/program/mongod/)</sup>

# MongoD Commands

| command | short | description |
| --- | --- | --- |
| `--help` | `-h` | show usage information |
| `--version` |  | show version information |
| `--config <file>` | `-f <file>` | specifies a configuartion file |
| `--auth` |  | enables authentication |
| `--noauth` |  | disables authentication |

## Edit /etc/mongo.conf

| command | short | description |
| --- | --- | --- |
| `--dbpath <path>` |  | specifies the directory for datafiles (default: /data/db) |
| `--logpath` |  | specifies the directory for logfiles (default: /var/log/mongodb/mongod.log)
| `--port <port-nr>` |  | specifies the port-number (default: 27017) |
| `--bind_ip [<ip_addr>, <ip_addr>]` |  | specifies which IP address should bind to (default: localhost) |
