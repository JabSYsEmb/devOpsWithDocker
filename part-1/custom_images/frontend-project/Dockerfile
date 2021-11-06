FROM node:14

WORKDIR /home/app/

COPY ./frontend .

EXPOSE 5000

RUN npm install

RUN npm run build

RUN npm install -g serve

CMD ["serve","-s","-l","5000","build"]
