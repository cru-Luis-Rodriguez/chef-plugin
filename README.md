perl-plugin
===========

run chef-client remotely under Jenkins CI. 
- chef json file generated from custom ERB template
- ssh public-key authentication schema is used

prerequisites
===
- ssh client

exported publishers
===

## chef_publisher

![layout](https://raw.github.com/melezhik/chef-plugin/master/images/layout.png "layout")

### chef json custom template
If you define one, chef_publisher will generate chef json file, based on the template. 
 - Check out chef wiki to get know about chef json files.
 - You can use ERB constructions here

### run chef client in remote host
chef-client will be run on remote server with chef json file generated.

## LC_ALL
Setup your standard encoding.

    ru_RU.UTF-8






