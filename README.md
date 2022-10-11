# Le réseau est en 172.16.1.0/24.

### Le découpage symétrique

- Le Pôle informatique (6 bureaux, environ 50 équipements au total)
Le Pôle développement (6 bureaux, environ 12 équipements au total)
Le Pôle Administratif (4 bureaux, environ 20 équipements au total)
Le Pôle Technicien (4 bureaux, environ 15 équipements au total)

Au moins 50 équipements pour chacun 
donc 2 puissance 6 = 64
64-2= 62 machines max par sous réseau
cidr=(62-6)=56


Le premier réseau Pôle informatique commencera à : 172.16.1.1 jusqu'à 172.16.1.62
L'adresse réseau de ce dernier sera : 172.16.1.0/56
L'adresse de broadcast de ce dernier sera : 172.16.1.63

Le deuxième réseau Pôle développement commencera à : 172.16.1.65 jusqu'à 172.16.1.126
L'adresse réseau de ce dernier sera : 172.16.1.64/56
L'adresse de broadcast de ce dernier sera : 172.16.1.127

Le troisième réseau Pôle Administratif commencera à :172.16.1.129 à 172.16.1.190
L'adresse réseau de ce dernier sera :  172.16.1.128/56
L'adresse de broadcast de ce dernier sera : 192.168.0.191

Et enfin le dernier réseau Pôle Technicien commencera à : 192.168.0.170 à 192.168.0.241
L'adresse réseau de ce dernier sera : 192.168.0.169/27
L'adresse de broadcast de ce dernier sera : 192.168.0.242


### Le découpage asymétrique

- Le Pôle informatique (6 bureaux, environ 50 équipements au total)
Le Pôle développement (6 bureaux, environ 12 équipements au total)
Le Pôle Administratif (4 bureaux, environ 20 équipements au total)
Le Pôle Technicien (4 bureaux, environ 15 équipements au total)


Le premier réseau Pôle informatique commencera à : 172.16.1.1 jusqu'à 172.16.1.62
L'adresse réseau de ce dernier sera : 172.16.1.0/56
L'adresse de broadcast de ce dernier sera : 172.16.1.63

Le deuxième réseau Pôle développement commencera à : 172.16.1.65 jusqu'à 172.16.1.78
L'adresse réseau de ce dernier sera : 172.16.1.64/12
L'adresse de broadcast de ce dernier sera : 172.16.1.79

Le troisième réseau Pôle Administratif commencera à :172.16.1.81 à 172.16.1.110
L'adresse réseau de ce dernier sera :  172.16.1.80/56
L'adresse de broadcast de ce dernier sera : 192.168.0.111

Et enfin le dernier réseau Pôle Technicien commencera à : 192.168.0.113 à 192.168.0.142
L'adresse réseau de ce dernier sera : 192.168.0.112/27
L'adresse de broadcast de ce dernier sera : 192.168.0.142

