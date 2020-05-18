FROM node:lts-alpine as test-env
WORKDIR /app
RUN apk add git && git clone https://github.com/ahfarmer/calculator.git && \
      cd calculator && npm install 
WORKDIR /app/calculator
EXPOSE 3000
CMD ["npm", "start"]
