FROM node:18-slim
WORKDIR /app
COPY ../tp1/package*.json ./
RUN npm install --only=production
COPY ../tp1/ ./
RUN npx tsc index.ts
EXPOSE 4040
CMD ["node", "index.js"]
