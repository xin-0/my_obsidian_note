# pip
PyPi
## env
Use `conda activate` and `conda deactivate` to switch in and out of [[conda]] env
Use `which pip` to see the pip in use

---
## change source
config file path when conda is ==activated==: `~/.config/pip/pip.conf`
### use command line
```bash
$ pip config set global.index-url https://<source>
$ pip config set install.trusted-host https://<source>
```


### Modify the config file
Modify the file as following
```text
[global]

index-url = <source>

[install]

trusted-host = <source>
```

---
## set proxy
conclusion for now:
can't set proxy for `pip` in conda virtual env
If want to install package in conda env, recommand `conda install` 