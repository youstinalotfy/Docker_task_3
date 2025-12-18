# استخدام Node.js كـ base image
FROM node:18-alpine

# تحديد مجلد العمل داخل الـ container
WORKDIR /app

# نسخ package.json و package-lock.json
COPY package*.json ./

# تنصيب الـ dependencies
RUN npm install

# نسخ باقي الملفات
COPY . .

# فتح البورت
EXPOSE 3000

# تشغيل التطبيق
CMD ["node", "server.js"]