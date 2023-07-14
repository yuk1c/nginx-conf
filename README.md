## Nginx configuration to speed up static websites and protect against Layer7 DDoS attacks.

### 📥 Installation
Clone the repository: <code>git clone https://github.com/yuk1c/nginx-conf</code>

Now stop your nginx: <code>sudo systemctl stop nginx</code>

Then rename your nginx config and replace it with our config (but before this we need root rights): <code>cd /etc/nginx/ && mv nginx.conf nginx.old && mv ~/nginx-conf/nginx.conf $PWD</code>

And now, you can start nginx again: <code>sudo systemctl start nginx</code>

### ⚙️ Configuration
All that you need - replace the worker_processes to <code>your cpu threads * 2</code>
If you want, you can configure SSL. 

### 📋 Requirements
- Ubuntu 20.04 or later
- Nginx (we recommend latest stable version)
- Apache2 running on 8080 port
- Cloudflare
