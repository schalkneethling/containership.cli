---
command-name: 'remote add'
permalink: '/docs/commands/remote-add'
---

<h2> {{ page.command-name }} </h2>

The `{{ page.command-name }}` command allows you to add a CLI remote pointing to a Containership cluster.

`csctl remote add <remote_name> <remote_url>`

|------+----+------------+----+----------|
| Argument | Alias | Description | Required | Default |
|-----------------|------|-----------|----------------|-------|
| remote_name | | Name of the remote for local reference | y | |
| remote_url | | URL of one of the `leader` nodes on your cluster | y | |
|=================+============+=================+================+===|

> This cluster will also need firewall rules for the Containership API open to the machine you are using the CLI from.
See <https://docs.containership.io/access-control/firewalls/oss-firewall-guidelines> for more information.
