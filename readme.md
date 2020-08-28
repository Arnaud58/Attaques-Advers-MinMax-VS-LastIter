# Génération d'images adverses et apprentissage robuste

Ce répo contient le travail mon stage de fin d'études. Celui-ci consiste à comparer la précision et la robustesse de deux réseaux entrainer avec deux méthodes différentes.

La première méthode est une méthode "MinMax" qui est développée par Solène Bernard pour la stéganographie.

La seconde méthode est une méthode ["Last-Iter"](https://arxiv.org/pdf/1706.06083.pdf) qui est développée par Madry pour les attaques adverses.

Il a été décider d'essayer ces méthodes avec deux types d'attaque différente FGSM et PGD.

Chaque fichier *.ipynb* contient une implémentation de la méthode faite avec une attaque différente, pour un total de quatre fichiers. Le nom de chaque fichier contient le nom de la méthode et de l'attaque utilisé tel que *methode_attaque.ipynb*.

Les attaques adverses sont générées via la librairie foolbox dans sa version 2.4. Ci-jointe la documentation de foolbox pour [FGSM](https://foolbox.readthedocs.io/en/v2.4.0/modules/attacks/gradient.html#foolbox.attacks.GradientAttack) et [PGD](https://foolbox.readthedocs.io/en/v2.4.0/modules/attacks/gradient.html#foolbox.attacks.L2BasicIterativeAttack).