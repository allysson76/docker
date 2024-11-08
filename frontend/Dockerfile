# Etapa 1: Usar a imagem oficial do Node.js com Alpine (mais leve)
FROM node:14-alpine

# Diretório de trabalho dentro do contêiner
WORKDIR /app

# Copiar package.json e package-lock.json (para otimizar a instalação de dependências)
COPY package*.json ./

# Instalar as dependências
RUN npm install

# Copiar todos os arquivos da aplicação React
COPY . .

# Build da aplicação React para produção
RUN npm run build

# Expor a porta onde a aplicação vai rodar
EXPOSE 3000

# Comando para iniciar a aplicação React
CMD ["npm", "start"]
