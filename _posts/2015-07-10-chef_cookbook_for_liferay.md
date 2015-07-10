---
layout: post
title:  "Chef Cookbook for Liferay"
date:   2015-07-10 16:11:00
categories: devops
tags: featured
#image: /assets/article_images/gopher.jpeg
comments: true
---

A chef cookbook for liferay in-memory db version.
Runs on precise64 3.2.0-23-generic Vagrant image

- [Liferay Cookbook in Chef Supermarket ](https://supermarket.chef.io/cookbooks/liferay)

- [Cookbook source](https://github.com/ganeshramr/my-chef-repo/tree/master/cookbooks/liferay)

8 Steps for quick run

1. Vagrant up the following box
<script src="https://gist.github.com/ganeshramr/0544c678e879bc580faa.js"></script>

2. ssh onto the box and ```sodo su```
3. Install chef client ```curl -L https://www.chef.io/chef/install.sh | sudo bash```
4. Verify installation by running ```knife```
5. (OPTIONAL) override your cookbook location for knife through ```knife.rb``` if required
6. run ```knife cookbook site install liferay```
7. run ```chef-client -z -o liferay```
8. give it sometime. launch http://192.168.33.12:8085/liferay-portal/ from your host
