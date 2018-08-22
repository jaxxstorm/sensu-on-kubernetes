# Sensu on Kubernetes

This repo serves as an example for running Sensu 1.x on Kubernetes

# Components

Sensu requires a [transport layer](https://docs.sensu.io/sensu-core/1.0/reference/transport/) for its operation. In this particular case, the transport is Redis. 

When using stateful services, its generally a good idea to use an [operator](https://coreos.com/operators/). I've chosen to use the wonderful [redis operator from spotathome](https://github.com/spotahome/redis-operator).

The rest of the components are the basic sensu building blocks, the API, server and client.

# Docker

The container container is located [here](https://github.com/jaxxstorm/docker-sensu) and bundles a bunch of the sensu kubernetes plugins with it.
