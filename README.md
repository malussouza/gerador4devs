# gerador4devs
Este repositório contém uma API simples para gerar dados fictícios utilizando o serviço fornecido pelo site 4Devs.

# Funções suportas pela API

- GERADORES


- [x] Gerador de CNH
- [x] Gerador de Conta Bancária
- [x] Gerador de CPF
- [x] Gerador de RENAVAM
- [x] Gerador de Veículos
- [x] Gerador de CNPJ
- [x] Gerador de CEP
- [x] Gerador de RG
- [x] Gerador Inscrição Estadual
- [x] Gerador Cartão de Crédito
- [x] Gerador de Pessoas
- [x] Gerador de Empresas
      
- VALIDADORES

- [x] Validador Cartão Crédito
- [x] Validador Conta Bancária
- [x] Validador de Certidões
- [x] Validador de CNH
- [x] Validador de CNPJ
- [x] Validador de CPF
- [x] Validador de PIS/PASEP
- [x] Validador de RENAVAM
- [x] Validador de RG
- [x] Validador Título de Eleitor
- [x] Validar Inscrição Estadual

## Pre Requisitos
Ter instalado: 
- [x] Docker
- [x] Postman
- [x] Node Js
- [x] nodemon

## Intalação

Para rodar localmente e necessario node js  11 <

- Faça o Download do repositorio

```sh
git clone 
```

- Instala as dependencias abrindo uma aba do terminal a partir da pasta

```sh
cd /src
npm install
```

## Dockerfile

Iniciar o projeto atraves do docker

- Gerar Build

```sh
docker build -t deividoliver/devtools .
```

- Run

```sh
docker run --rm -p 3000:3000 deividoliver/devtools
```

- Docker composer

Utilize o docker composer para iniciar a api no modo desenvolvedor
onde sera iniciado com o nodemon e as alterações no código sera aplicada em tempo real.

```sh
docker-compose up
```

## Postman

Importe o json do postman para auxiliar nos endpoints disponiveis

Pode criar suas massas de testes


