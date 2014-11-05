lxc-ps2
=======

lxc-ps2 is a wrapper of the 'ps' command that can show
the names of the lxc VMs that processes are running in.

lxc-ps2 behaves identically to the 'ps' command except
that it adds support the following format specifiers:

    ipcnsn, mntnsn, netnsn, pidnsn, usrnsn, utsnsn

which will list the respective lxc VM names in which a
process is running.

The [lxc project itself](https://github.com/lxc/lxc) had
a [lxc-ps implementation][https://github.com/lxc/lxc/blob/0306de4f280adc0cd5faa3cd365c584d61c9e383/src/lxc/lxc-ps.in]
which [was removed](https://github.com/lxc/lxc/commit/7f12cae956c003445e6ee182b414617b52532af6).

There was a virt-ps tool by Richard W.M. Jones floating
around once, but that also seems to have been dropped.

lxc-ps2 is implemented in shell and is very rough, but
it could certainly be improved and it could also be
extended to other namespace based virtualisation
techniques like f.ex.
[docker](https://duckduckgo.com/l/?kh=-1&uddg=https%3A%2F%2Fwww.docker.com%2F).
