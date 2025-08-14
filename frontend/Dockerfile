FROM node:14-alpine

WORKDIR /app

COPY package.json ./
RUN npm install

COPY . .

# Let React run inside Docker
ENV HOST=0.0.0.0

EXPOSE 3000
CMD ["npm", "start"]
