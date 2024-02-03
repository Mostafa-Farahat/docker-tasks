FROM node:21-alpine3.18

COPY package*.json /app/
COPY src /app/

WORKDIR /app

RUN npm install

CMD ["node", "app.js"]

# fault 1: the FROM should be first line file and use an image that has node
# fault 2: the COPY clauses should be before the npm install
# fault 3: the /app direcotry should be /app/ so that docker creates the
#          the directory if it doesn't exist and RUN should be a CMD caluse 