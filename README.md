## Introdução

Uma ferramenta de código livre, o nmap (Network Mapper) é utilizado para mapeamento de redes. Suas principais funcionalidades são: identificação de sistemas operacionais, varredura de portas e detecção de versões de serviços. Criada por Gordon Lyon.
Usada principalmente para testes de invasão e firewall. Funciona por envio de pacotes e analisa as respostas recebidas.
O código fonte pode ser encontrado no github: https://github.com/nmap/nmap

Instalando o nmap

Linux: 
```
 apt install nmap
```

Mac:
```
brew install nmap
```
ou baixando o .dmg no site oficial: https://nmap.org/download.html

------------------------------------------------------------------------------------------------------------

Escaneando portas:
```
nmap scanme.nmap.org -p80
nmap scanme.nmap.org -p443
```
![Listagem de portas especificas](https://raw.githubusercontent.com/biridiz/Tutorial-nmap/main/images/lista-portas.png)

------------------------------------------------------------------------------------------------------------
Listando portas:
```
nmap scanme.nmap.org
```

![Listagem de portas especificas](https://raw.githubusercontent.com/biridiz/Tutorial-nmap/main/images/lista.png)

------------------------------------------------------------------------------------------------------------
Identificando o sistema operacional:
```
nmap -O scanme.nmap.org
```

![Listagem de portas especificas](https://raw.githubusercontent.com/biridiz/Tutorial-nmap/main/images/os.png)

------------------------------------------------------------------------------------------------------------
Detectando versões:
```
nmap -sV scanme.nmap.org
```

![Listagem de portas especificas](https://raw.githubusercontent.com/biridiz/Tutorial-nmap/main/images/versoes.png)

------------------------------------------------------------------------------------------------------------
Filtrando por protocolos:

TCP:
```
nmap -sT scanme.nmap.org
```
UDP:
```
nmap -sU scanme.nmap.org
```

![Listagem de portas especificas](https://raw.githubusercontent.com/biridiz/Tutorial-nmap/main/images/tcp-udp.png)

------------------------------------------------------------------------------------------------------------
Mostrando rotas e interfaces:
```
nmap -iflist
```

![Listagem de portas especificas](https://raw.githubusercontent.com/biridiz/Tutorial-nmap/main/images/rotas.png)

------------------------------------------------------------------------------------------------------------

