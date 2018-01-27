# Dockerhub üzerinden resmi Node 8 image'ını temel alarak bir image oluştur
FROM node:8

# Uygulamamızın bulunacağı klasörü oluştur
RUN mkdir -p /var/www/app

# Komutlarınızın çalıştırılacağı dizini seç
WORKDIR /var/www/app

# package.json dosyamızı çalışma dizinine kopyala
COPY package.json /var/www/app

# Bağımlılıkları kur
RUN npm install

# Tüm proje dosyalarını docker image'ına kopyala
COPY . /var/www/app

# Uygulamanın çalışacağı port
EXPOSE 4200

# Projeyi ayağa kaldıracak komutu çalıştır
CMD ["npm", "start"]