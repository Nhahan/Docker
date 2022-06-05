FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

CMD ["node", "server.js"]

# docker build -t feedback-node . // 태그를 feedback-node로
# docker run -p 3000:80 -d --rm feedback-node // -p:내부 포트 80을 외부 포트 3000으로 연결하고, -d:detach모드로 실행해서 바로 터미널로 가게끔하고, --name 이름을 feedback-app으로 설정, --rm 컨테이너 종료 후 자동종료
# docker ps // 컨테이너 목록