FROM node:18-alpine

WORKDIR /app

ARG REACT_APP_RAZORPAY_KEY_ID
ENV REACT_APP_RAZORPAY_KEY_ID=$REACT_APP_RAZORPAY_KEY_ID

COPY package*.json ./
RUN npm install

COPY . .

# Expose your specific port
EXPOSE 5000

# Start command
CMD ["npm", "run", "start"]