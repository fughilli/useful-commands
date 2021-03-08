# Useful Shell Commands

## Generate a 2048-bit SSH RSA keypair and save it to `id_rsa{,.pub}`

`ssh-keygen -N "" -t rsa -b 2048 -f id_rsa`

## Setup passwordless login for a remote host

`cat ~/.ssh/id_rsa.pub | ssh <user>@<host> "mkdir -p ~/.ssh; cat - >> ~/.ssh/authorized_keys"`
