1. Mesure et Observation :
    - docker stats:
        CONTAINER ID   NAME          CPU %     MEM USAGE / LIMIT     MEM %     NET I/O           BLOCK I/O        PIDS
        0ee5c8f5537e   catalog-api   0.02%     64.99MiB / 15.53GiB   0.41%     24.6kB / 17.8kB   0B / 0B          32
        9997f60de8d2   catalog-db    1.66%     1.087GiB / 15.53GiB   7.00%     12.3kB / 11.8kB   1.21GB / 117MB   254

        - Le conteneur catalog-db (Database) consomme massivement des ressources RAM CPU et NET I/O tant que le conteneur catalog-api de l'API est trés léger et consomme 0B sur le disque (pas besoin de persistance )
        - Importance de la mesure :
            -- La mesure nous aide a detecter les défaillances et anomalies pour prévenir les pannes severes dans un systeme .
        - Pour assurer le suivi dans une chaine on peut mesurer les métriques suivants:
            - temps de réponse des requetes 
            - taux d'utilsation des ressources par nos services
            - 
          