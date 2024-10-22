#使用 node.js 作為 base Image
FROM node:16

#於容器內創建資料夾
RUN mkdir -p /usr/src/app

#指定工作目錄
WORKDIR /usr/src/app

#將dockerfile目錄底下所有東西複製到 app
COPY . /usr/src/app

#執行npm指令來下載package.json中，所寫入的依賴元件
RUN npm install

#將 8080 port 映射到主機
EXPOSE 8080

#執行node指令指定設定檔運行web server
CMD ["node","server.js"]

