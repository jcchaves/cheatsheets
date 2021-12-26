# SSH

## Keygen

Generating a RSA key pair for use when interacting with servers or service providers using SSH:

- No passphrase

```sh
ssh-keygen -t rsa -N "" -f <path to key pair files>
```

- With passphrase

```sh
ssh-keygen -t rsa -N "my-passphrase" -f <path to key pair files>
```

## Verify SSH key pair passphrase

Use the option __*-y*__ to view the public key assocaited to the generated key pair. It will request the passphrase if set.

From the __*man*__ page:

> This option will read a private OpenSSH format file and print an OpenSSH public key to stdout.

```sh
ssh-keygen -y -f <path to key pair file>
```
