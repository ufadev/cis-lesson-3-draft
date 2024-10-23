FROM node:22

COPY ["src/package.json", "src/package-lock.json", "./"]
RUN npm ci

COPY src/ .
RUN npm run build

CMD ["npm", "start"]

# docker build -f Dockerfile -t lesson2 ../