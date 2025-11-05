# Lab5-GEI311-SBIR

Réponses aux questions : 
- Q6 : L'application étant arrêté, on remarque qu'il n'est maintenant plus possible d'accèder à http://IP_DE_LA_MACHINE:3000/. C'est logique puisque le "serveur" est stoppé.

- Commandes utiles nginx : 
    - nginx -s stop	= fast shutdown
    - nginx -s quit = graceful shutdown
    - nginx -s reload = changing configuration, starting new worker processes with a new configuration, graceful shutdown of old worker processes
    - nginx -s reopen = re-opening log files