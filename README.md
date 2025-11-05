# Lab5-GEI311-SBIR

# Informations
Projet développé pour le cours GEI311 - Architecture Logicielle

PAR : Il'aina Ratefinanahary et Samuel Brassard UQAC - Automne 2025

*Ce projet est à usage éducatif uniquement*

# Objectif
Ce laboratoire a pour objectif "l'initiation aux notions liées au déploiement et la distribution de charge."

# Ce que nous avons appris dans ce laboratoire
Lors de ce laboratoire, nous avons appris à effectuer le déploiement d'une application simple mais surtout à utiliser la distribution de charge
pour cette application.

# Commandes utiles
- tasklist /fi "imagename eq nginx.exe" = Voir si nginx est actuellement exécuté
- start nginx = démarrer nginx
- nginx -s stop	= fast shutdow
- nginx -s quit = graceful shutdown
- nginx -s reload = changing configuration, starting new worker processes with a new configuration, graceful shutdown of old worker processes
- nginx -s reopen = re-opening log files

# Réponses aux questions
- Q6 : L'application étant arrêté, on remarque qu'il n'est maintenant plus possible d'accèder à http://IP_DE_LA_MACHINE:3000/. C'est logique puisque le "serveur" est stoppé. La manipulation effectuée pour obtenir ce résultat était simplement de fermer l'invite de commande exécutant l'application.   

- Q16 : 

- Q17 :
    - a. 
    - b. 