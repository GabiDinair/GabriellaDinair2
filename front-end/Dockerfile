# Usando a imagem base do Node.js
FROM node:14-alpine

# Diretório de trabalho
WORKDIR /app

# Copiar os arquivos de dependências
COPY package*.json ./

# Instalar dependências
RUN npm install

# Copiar o código fonte
COPY . .

# Construir a aplicação React
RUN npm run build

# Expor a porta do React (3000)
EXPOSE 3000

# Comando para iniciar o servidor
CMD ["npm", "start"]
