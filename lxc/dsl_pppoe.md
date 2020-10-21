#lxc
#lxd
#pppoe
#linux.kernel_modules
#kernel_modules
#device
#config
```bash
lxc config device add <container> ppp unix-char path=/dev/ppp
lxc config set <container> linux.kernel_modules pppoe
```

#error
> if pppoe kernel_module not enabled
```bash
> Couldn’t open the /dev/ppp device: Operation not permitted
> Sorry - this system lacks PPP kernel support
```
