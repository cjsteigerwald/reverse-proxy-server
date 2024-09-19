# reverse-proxy-server
This is a reverse proxy server running in the cloud via Docker

Need to create following empty files
logs/ws/traefik/access.log
logs/ws/traefik/traefik.log
appdata/traefik3/acme/acme.json

Create and add following files in secrets folder:
basic_auth_credentials
cf_dns_api_token
zero_tier_network_id

Following in .env:
PUID=1000
PGID=1000
TZ="America/Los_Angeles"
USERDIR="<user_home_dir>"
DOCKERDIR="<docker_home_dir>"
HOSTNAME="<server_host_name>"
SERVER_IP=<server_public_ip>
LOCAL_IPS=127.0.0.1/32,10.0.0.0/8,192.168.0.0/16,172.16.0.0/12
DOMAINNAME_1=<fqdn>
LOCAL_IPS=127.0.0.1/32,10.0.0.0/8,192.168.0.0/16,172.16.0.0/12
CLOUDFLARE_IPS=173.245.48.0/20,103.21.244.0/22,103.22.200.0/22,103.31.4.0/22,141.101.64.0/18,108.162.192.0/18,190.93.240.0/20,188.114.96.0/20,197.234.240.0/22,198.41.128.0/17,162.158.0.0/15,104.16.0.0/13,104.24.0.0/14,172.64.0.0/13,131.0.72.0/22
ZERO_TIER_NETWORK_ID=<zero_tier_network_id>
HOME_SERVER_IP=<zero_tier_home_network_ip>

