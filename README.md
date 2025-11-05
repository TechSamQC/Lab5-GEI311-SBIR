# Lab5-GEI311-SBIR

# Informations
Projet développé pour le cours GEI311 - Architecture Logicielle
par Il'aina Ratefinanahary et Samuel Brassard UQAC - Automne 2025
*Ce projet est à usage éducatif uniquement*

# Introduction
Ce laboratoire a pour objectif "[l'i]nitiation aux notions liées au déploiement et la distribution de charge."

# Ce que nous avons appris dans ce laboratoire


# Réponses aux questions
- Q6 : L'application étant arrêté, on remarque qu'il n'est maintenant plus possible d'accèder à http://IP_DE_LA_MACHINE:3000/. C'est logique puisque le "serveur" est stoppé. La manipulation effectuée pour obtenir ce résultat était simplement de fermer l'invite de commande exécutant l'application.

- Commandes utiles nginx :
    - tasklist /fi "imagename eq nginx.exe" = Voir s'il est actuellement exécuté
    - start nginx = démarrer
    - nginx -s stop	= fast shutdow
    - nginx -s quit = graceful shutdown
    - nginx -s reload = changing configuration, starting new worker processes with a new configuration, graceful shutdown of old worker processes
    - nginx -s reopen = re-opening log files

- Q16 : 

- Q17 :
    - a. 
    - b. 