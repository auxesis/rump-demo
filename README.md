rump-demo manifests
===================

modules/ <= Puppet modules
manifests/ <= Puppet nodes
vendor/ <= frozen Puppet + Facter

Running Puppet with Rump
------------------------

From within this directory, run:

    rump go

You can pass options to Puppet after the 'go':

    rump go --debug --test

Freezing Puppet
---------------

Firstly, you need to create a git repository:

    git init

Now you can freeze Puppet:

    rump freeze

Now Rump will use the frozen Puppet when you run 'rump go'.

