# mi-core-base

This repository is based on [Joyent mibe](https://github.com/joyent/mibe).

## description

Minimal 0x61 mibe image

## mdata variables

### admin authorized_keys

Configure ssh public key for admin user via `mdata` variable.

- `admin_authorized_keys`: ssh public key for the admin user

### root authorized_keys

Configure ssh public key for root user via `mdata` variable.

- `root_authorized_keys`: ssh public key for the root user

### root ssh public private key

Configure ssh public and private key pair for root user via `mdata`. We only
support rsa keys.

- `root_ssh_rsa`: private ssh rsa key for root user
- `root_ssh_rsa_pub`: public ssh key for root user (mostly not required)

### ssh daemon

Configure ssh public and private key pairs for the host daemon via `mdata`.

- `ssh_host_rsa_key`:     private SSH rsa key
- `ssh_host_rsa_key.pub`: public SSH rsa key
- `ssh_host_dsa_key`:     private SSH dsa key
- `ssh_host_dsa_key.pub`: public SSH dsa key

