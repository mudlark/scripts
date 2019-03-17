# Guest script and service

There are two files in this directory. Unless you are altering the service file, the script `set-hostname` needs to be placed in the `/root` directory of the base VM guest image

You can add the `set-hostnmae.service` file to your favorite systemd config location (I use `/etc/systemd/system`)


After that, run: 
```
$ systemctl daemon-reload
$ systemctl enable set-hostname
```


See https://beyondthekube.com/my-lab-setup/ for more details about setting this up.
