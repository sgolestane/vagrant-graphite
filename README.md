vagrant-graphite
=======================

# graphite to go

Provision graphite in a virtual machine with vagrant and puppet

## Details:

 * port forwardings enabled
 * graphite: http://localhost:2000/

## Installation

```
git clone https://github.com/sgolestane/vagrant-graphite.git
cd vagrant-graphite-puppet
librarian-chef install
vagrant up
open http://localhost:2000/
```