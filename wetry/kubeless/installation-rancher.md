Pour installer Rancher, il vous suffit de démarrer un container Docker:

`sudo docker run -d --restart=unless-stopped -p 880:80 -p 8443:443 rancher/rancher`{{copy}}

*Attention à ne pas utiliser ni le port 80 ni le port 443 que nous réservons pour le load-balancer (Ingress).*

Vous aurez alors accès à votre Rancher à l'addresse suivante:

https://[[HOST_SUBDOMAIN]]-8443-[[KATACODA_HOST]].environments.katacoda.com
