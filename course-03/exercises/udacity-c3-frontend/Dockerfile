FROM beevelop/ionic

WORKDIR /usr/src/app

COPY . .

RUN npm install npm@latest -g
RUN npm install -g @angular/cli

COPY package*.json ./
RUN npm ci

EXPOSE 8100
CMD [ "ionic", "serve"] 