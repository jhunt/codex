Codex
=====

This repository houses notes that will one day turn into scripts
and a document on following The Codex Way (TM).

What Does It Do?
----------------

`codex` is an attempt to provide an assistant to ops folks who are
trying to follow The Codex Way (TM), by managing some of the
duller bits of implementing Codex.

To that end, the `codex` binary deals in _sites_ that allow you to
segregate one set of environments from another.

To get started, run `codex start lab`.  This will setup a lab site
for you to experiment with Codex.  Each site comes with a
single-instance, loopback-bound, file-backed Vault instance, which
`codex` will manage for you (sealing, authentication, etc.).

When you're done interacting with the "lab" site, you can spin it
(and its Vault) down with `codex stop lab`.  To start it back up
again, run `codex start lab`.  You can also spin down _all_ of
your Codex sites by simply issuing `codex stop`.

`codex sites` will give you a list of all of your configured
sites.

What Will It Do?
----------------

I have plans for `codex`.  Big plans.

In the future, `codex` will help manage your cloud-config and
runtime-configs using a common interface and a simplified file
format.  For example, the common case of cutting up a large
network into smaller, CIDR-coherent networks is something a tool
should do.  That tool can be `codex`.

In the future, `codex` will help you map out what you've got and
what you still need to deploy a complete Codex installation.  Do
you have SHIELD?  Are there concourse workers for each of your
environment BOSHes?  Did you deploy all the jumpboxen you need?o

In the future `codex` may even completely wrap Genesis, and let
you manage and deploy all of your systems and infrastructure from
a single git repository.  Who knows?
