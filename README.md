## PBX Project

Let's play with asterisk and see what's up.

## Dev Environment

This project offers two different development environments. One base
one virtualization, one based on containerization.

Why?

Because one of the contributor develops personnal projects on a box that
does not support containerization, the other contributor doesn't want
to live in the past.

### VirtualBox (using Vagrant)

To manage VirtualBox guest additions (not mandatory, but friendly):

```
vagrant plugin install vagrant-vbguest
```

Then, to provision and start the VM:

```
vagrant up --provision
```

### Docker (using cqfd)

Initialize the dev environment:

```
cqfd init
```

The default cqfd flavor will provision a PBX in development environment:

```
cqfd
```

