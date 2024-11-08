# Etapa 1: Usar a imagem oficial do Node.js
FROM node:14

# Diretório de trabalho dentro do contêiner
WORKDIR /app

# Copiar package.json e package-lock.json
COPY package*.json ./

# Instalar as dependências
RUN npm install

# Copiar todos os arquivos da aplicação
COPY . .

# Expor a porta do servidor (padrão Express)
EXPOSE 5000

# Comando para rodar a aplicação Express
CMD ["npm", "start"]
