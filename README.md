# local redis cluster setup

Create and start a local cluster with 6 redis-server's

    ./cluster <path to your redis src folder>

The redis instances will throw logs to /var/log/redis-cluster/. Please, be sure it exists and the redis process is able to write there, for example:

    mkdir /var/log/redis-cluster
    chown a+w /var/log/redis-cluster


Killall is your friend:

    killall -m redis-server

You may need to use `sudo` as the `redis` process runs as root.

