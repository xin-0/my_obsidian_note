## Proxy setting
edit ~/.condarc file as:

```text
# Show channel URLs when displaying what is going to be downloaded and
# in 'conda list'. The default is False.
show_channel_urls: true
allow_other_channels: true
  
proxy_servers:
	http: http://tongxin:2020Tx!@10.10.10.10:3128/
	https: http://tongxin:2020Tx!@10.10.10.10:3128/

# 设置verify=False移除SSL认证时，解决InsecureRequestWarning警告
ssl_verify: false
```