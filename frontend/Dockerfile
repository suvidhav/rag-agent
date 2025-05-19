FROM node:20

WORKDIR /app

COPY rag-agent/package*.json ./rag-agent/
WORKDIR /app/rag-agent
RUN npm install

COPY rag-agent/ /app/rag-agent/

RUN npm run build

EXPOSE 3000
CMD ["npm", "run", "start"]
