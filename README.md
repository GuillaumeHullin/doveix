# doveix
Zabbix Active Agent - Dovecot

    git clone https://github.com/GuillaumeHullin/doveix.git
    ./doveix/deploy_zabbix.sh
    systemctl restart zabbix-agent

You can use arguments like:
    
    ./doveix/deploy_zabbix.sh <DOVEIX_URI> <DOVEIX_USER> <DOVEIX_PASS> <CACHE_DIR> <CACHE_TTL>
 
You also need to create Dovecot user based on the data in ${ZABBIX_DIR}/zabbix_agentd.d/doveix.conf
Note that the password will be random if the default "xxxxxx" is used.
