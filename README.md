# Lab5-GEI311-SBIR

# Informations
Projet développé pour le cours GEI311 — Architecture Logicielle

PAR : Il'aina Ratefinanahary, Samuel Brassard et Antoine Larouche Tremblay UQAC — Automne 2025

*Ce projet est à usage éducatif uniquement*

# Objectif
Ce laboratoire a pour objectif «l’initiation aux notions liées au déploiement et la distribution de charge.»

# Ce que nous avons appris dans ce laboratoire
Lors de ce laboratoire, nous avons appris à effectuer le déploiement d’une application simple, mais surtout à utiliser la distribution de charge pour cette application.

# Commandes utiles
- tasklist/fi «imagename eq nginx.exe» = Voir si nginx est actuellement exécuté
- start nginx = démarrer nginx
- nginx -s stop	= fast shutdow
- nginx -s quit = graceful shutdown
- nginx -s reload = changing configuration, starting new worker processes with a new configuration, graceful shutdown of old worker processes
- nginx -s reopen = re-opening log files

# Réponses aux questions
- Q6 : L’application étant arrêtée, on remarque qu’il n’est maintenant plus possible d’accéder à http://IP_DE_LA_MACHINE:3000/. C’est logique puisque le «serveur» est stoppé. La manipulation effectuée pour obtenir ce résultat était simplement de fermer l’invite de commande exécutant l’application.

- Q16 : Lorsque nous avons activé nginx, nous avons dès lors remarqué qu’en rafraîchissant la page, l’adresse IP du membre A et du membre B s’alternent. C’est normal puisque nous sommes maintenant en train d’utiliser le load balancer (nginx). Celui-ci utilise alors un algorithme du tourniquet pour choisir le nœud.

- Q17 : La manipulation effectuée est la même qu’à la question 6.
    - a. Non, c’est le même cas que précédemment dans la question 6. Nous avons arrêté l’application du membre A, celle du port 3000 (en connexion directe) ne fonctionne plus.
    - b. Dans ce cas, oui, il est toujours possible d’accéder à l’application via le port 8181. L’adresse IP affichée est maintenant toujours celle du membre B, ce qui est logique puisque le load balancer redirige directement l’utilisateur vers le nœud fonctionnel. L’application du membre A n’est plus le single point of failure, c’est maintenant le load balancer. Si on avait arrêté celui-ci, l’application n’aurait plus été accessible.
