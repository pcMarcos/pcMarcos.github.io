---
layout: default
title: "How Jekyll works under the hood?"
date: 2023-02-27 17:05:00
categories: redis rails
---

If you're using Redis to [store your cache](https://guides.rubyonrails.org/caching_with_rails.html#activesupport-cache-rediscachestore) you can check how much memory is being consumed by the objects stored under a specific key.

You need to connect to your Redis container

`docker container exec -it {{container_id}} sh`

Check if your Redis implementation has more than one database. You can connect to the redis-cli for a specific DB with `redis-cli -n 2`


To list all keys you can run `keys *` or follow an specific pattern like `keys user*`.


You have the key you need, you can get the stored information in that key with 

`GET user_1_attributes`.


To get the memory usage of this object, use `memory usage user_1_attributes` and you'll have something like: 

`(integer) 1411` this number is measured in bytes.
