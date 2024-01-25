# Use a imagem base do Node.js 14 no Alpine Linux
FROM node:14-alpine3.14

# Define variáveis de ambiente
ARG NODE_ENV=development
ARG PORT=3000

ENV NODE_ENV=${NODE_ENV}
ENV PORT=${PORT}

# Define o diretório de trabalho no contêiner
WORKDIR /app

# Copia o arquivo package.json separadamente para aproveitar o cache de camadas do Docker
COPY ./src/package.json .

# Limpa o cache do npm
RUN npm cache clean --force

# Instala as dependências do projeto
RUN npm install

# Copia todos os arquivos do diretório de origem para o diretório de trabalho no contêiner
COPY ./src .

# Remove os arquivos desnecessários após a instalação das dependências
RUN rm -rf node_modules/.cache

# Expõe a porta definida
EXPOSE ${PORT}

# Comando para iniciar a aplicação
CMD ["npm", "run", "start"]
