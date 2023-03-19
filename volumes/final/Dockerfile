FROM node:alpine

WORKDIR /usr/app

COPY package.json .

RUN npm install

COPY . .

CMD ["npm", "run", "start"]

# Command to build the image 
# docker build -t my-reac-app-image .

# Command to run with 2 volumes
# docker run -v $(pwd):/usr/app -v /usr/app/node_modules -it --name my-reac-app-container -p 3000:3000 my-reac-app-image
