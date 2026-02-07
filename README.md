### Exposing to public
1. upload ngrok.sh to server
2. run ```chmod +x ngrok.sh```
3. run ```./scripts/ngrok.sh > /dev/null 2>&1 &```

### Backup
1. Run ```mkdir /home/gymbro/pgdata```
2. Run ```sudo chown -R 999:999 /home/gymbro/pgdata```
3. Run ```sudo chmod -R 700 /home/gymbro/pgdata```
4. Run ```mkdir /home/gymbro/n8ndata```

### SSL
1. Install certbot ```sudo apt-get install certbot python3-certbot-apache```
2. Generate certificate ```certbot certonly --standalone```
3. Add path to N8N_SSL_CERT and N8N_SSL_KEY 
4. N8N_SSL_CERT=/etc/letsencrypt/live/gymsbro.com/fullchain.pem 
5. N8N_SSL_KEY=/etc/letsencrypt/live/gymsbro.com/privkey.pem
