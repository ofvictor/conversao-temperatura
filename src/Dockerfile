FROM node:22.14.0
WORKDIR /app
# A cópia das dependências separada do código-fonte permite otimização da imagem
# quando apenas o código-fonte é alterado, sem necessidade de reinstalar as dependências 
COPY package*.json ./
RUN npm install
COPY . .
CMD ["node", "server.js"]