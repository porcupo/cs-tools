cs-tools
========

A few minor tools to pull information from cloudstack.

Instructions
------------
1. Run `bundle install`
2. copy `csconfig.yaml.example` to `csconfig.yaml`
3. configure api key, api secret, and url
4. Run `bundle exec <script> [params]`

Scripts
-------
First group of scripts are pretty self-explanatory; will list all available entries.
* listemplates
* listisos
* listnetworks
* listserviceofferings
* listvms 
* listzones

* searchvms: run `searchvms <string>` for a fuzzy string search of vms

Problems
--------
* Repeats itself a lot
* Should be broken down into classes vs. separate scripts
* Should also make some use of OOP
* Lacks any kind of testing
* pagination is only enabled for `listvms` and `searchvms`
