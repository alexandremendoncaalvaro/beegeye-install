# Beegeye | Instalacão Local  
## Prerequisitos  
![os](https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=white)  
![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg?logo=python&logoColor=white)  
![Poetry](https://img.shields.io/badge/poetry-gray.svg?logo=python&logoColor=white)  

## Instalação dos requisitos no WSL2 Ubuntu  
Segue um guia facilitado pra instalar os requisitos de forma automatizada com poucos comandos:  
https://github.com/alexandremendoncaalvaro/wsl-python-node

## Repositório do Beegeye
Pra facilitar criamos uma cópia da versão mais recente nesse local:
```Bash
https://anheuserbuschinbev-my.sharepoint.com/:f:/g/personal/alexandre_alvaro_ambevtech_com_br/Eu5V9Vda2cxAtXSrO3VuiLwBmdrEbWcD247g_tQX-iEPTw?e=gbOex6
```

Copie a pasta Beegeye para a raíz da pasta de usuário do Ubuntu.
Caso esteja usando o WSL o caminho pelo Windows Explorer é este:
```Bash
\\wsl$\Ubuntu\home\{nome de usuário}\
```
No Ubuntu fica assim:
```Bash
~/Beegeye
```

## Executando o Beegeye  
### Na primeira vez:  
*Use a senha criada para o Ubuntu caso necessário.  
Garanta q está no diretório do Beegeye:  
```Bash
cd ~/Beegeye
```

```Bash
cp example.env .env && sudo apt install ffmpeg -y && sudo chmod +x ./run-local.sh && poetry install
```

### Sempre que for rodar: 
Garanta q está no diretório do Beegeye:  
```Bash
cd ~/Beegeye
```
Carregue o ambiente virtual do python:  
```Bash
poetry shell
```
Rode a aplicação:  
```Bash
./run-local.sh
```
Abra um navegador de internet no Windows no endereço:
```Bash
localhost:5000
```

## Problemas na instalação  
Se durante a instalação ocorrer algum problema pra baixar bibliotecas ou algo do tipo, tente mudar o seu DNS.  
Sugestões de DNS: 1.1.1.1 ou 8.8.8.8
