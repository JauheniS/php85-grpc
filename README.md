# PHP 8.5 gRPC
PHP 8.5 Dockerfile to build with gRPC and Protobuf

# What's inside?
## Dockerfiles AMD64
- Dockerfile for Debian
- Dockerfile for Alpine

# Why this exists?
## To send this to the server and compile

This package is used to compile PHP container that could be used as FROM instead of official PHP 8.5 repository.
Why would you want that? gRPC compilation is taking many resources or more than 15 minutes of time, and sometimes you need this pre-compiled

You are welcome to pull-request your versions here.

# Contribution
## WARNING! This repository is not meant to install anything except of PHP and gRPC
- Do not overload your Dockerfile with other tech (RoadRunner, MongoDB, AMQP, etc). User would install this after with no problem
- For PHP 8.5 it must have PIE installed, watch the guides on how to do that
- You may use PECL - for now that's not the problem, but if it goes full-deprecated by PHP - your file would be removed from new release.
