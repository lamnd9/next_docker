FROM node:18-alpine

# Thư mục làm việc trong container
WORKDIR /app

# Copy file cấu hình package
COPY package.json package-lock.json ./

# Cài dependency
RUN npm install

# Copy toàn bộ mã nguồn vào container
COPY . .

# Mở cổng mặc định của Next.js
EXPOSE 3000

# Lệnh khởi chạy dev server
CMD ["npm", "run", "dev"]
