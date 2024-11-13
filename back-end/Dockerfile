# Usando a imagem base do Node.js
FROM node:14

# Diretório de trabalho
WORKDIR /app

# Copiar os arquivos de dependências
COPY package*.json ./

# Instalar dependências
RUN npm install

# Copiar o código fonte
COPY . .

# Expor a porta do Express (5000)
EXPOSE 5000

# Comando para iniciar o servidor Express
CMD ["npm", "start"]
