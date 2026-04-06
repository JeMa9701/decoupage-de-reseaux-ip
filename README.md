# **DECOUPAGE SYMETRIQUE**  

|               | Adresse réseau | Adresse broadcast | Adresse de début de plage | Adresse de fin de plage |
|:--------------|:---------------|:------------------|:--------------------------|:------------------------|
|Le Pôle informatique    |172.16.1.0/26  |172.16.1.63   |  172.16.1.1 | 172.16.1.62  |
|Le Pôle développement   |172.16.1.64/26 | 172.16.1.127 | 172.16.1.65 | 172.16.1.126 |
|Le Pôle Administratif   |172.16.1.128/26 | 172.16.1.191 | 172.16.1.129  | 172.16.1.190 |
|Le Pôle Technicien      |172.16.1.192/26 | 172.16.1.255 |  172.16.1.193 | 172.16.1.254 |  

### Le pole informatique étant le pole avec le plus d'équipements je prends celui-ci pour calculer mon découpage symetrique donc je le coupe en 4 sous réseaux ce qui me donne 2^6 donc 64 adresses par sous-réseau en enlevant l'adresse de réseau et celle de broadcast 62 adresses sont disponibles pour chaque sous-réseau


# **DECOUPAGE ASYMETRIQUE**
|               | Adresse réseau | Adresse broadcast | Adresse de début de plage | Adresse de fin de plage |
|:--------------|:---------------|:------------------|:--------------------------|:------------------------|
|Le Pôle informatique|172.16.1.0/26  |172.16.1.63   |  172.16.1.1 | 172.16.1.62  |
|Le Pôle développement|172.16.1.64/28|172.16.1.80| 172.16.1.65|172.16.1.79|
|Le Pôle Administratif|172.16.1.81/27|172.16.1.113|172.16.1.82|172.16.1.112|
|Le Pôle Technicien|172.16.1.114/27|172.16.1.146|172.16.1.115|172.16.1.145|

**Le pole informatique**: Environ 50 équipements;  2^6-2 = 64 donc de 0 a 64 en /26

**Le pole développement**: Environ 12 équipements; 2^4-2 = 14 donc de 64 a 80 en /28

**Le pole Administratif**: Environ 20 équipements; 2^5-2 = 30 donc de 81 a 113 en /27

**Le pole Technicien**: Environ 15 équipements; 2^5-2 = 30 donc de 114 a 146 en /27
