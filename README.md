# 🛒 Simple MERN Project – Ürün Ekleme ve Listeleme Uygulaması

Bu proje, temel bir **MERN** (MongoDB, Express.js, React, Node.js) yapısının **MongoDB içermeyen** sade bir versiyonudur. Kullanıcılar ürün adı ve fiyat girerek yeni ürünler ekleyebilir; mevcut ürünler arayüzde listelenir.

> Not: Veriler şu an sadece sunucu belleğinde tutulmaktadır (`DUMMY_PRODUCTS`). Gerçek bir veritabanı bağlantısı yoktur.

---

## 📦 Teknolojiler

- 💻 **Frontend**: React + Fetch API
- 🌐 **Backend**: Express.js + body-parser
- 🧠 **Veri**: Geçici dizi (`DUMMY_PRODUCTS`)
- 🔄 **API**: RESTful GET ve POST endpoint’leri

---

## 🚀 Kurulum ve Çalıştırma

### 1. Backend'i Başlat

```bash
cd backend
npm install
node server.js
```

Sunucu `localhost:5000` adresinde çalışır.

### 2. Frontend'i Başlat

```bash
cd frontend
npm install
npm start
```

Uygulama `localhost:3000` üzerinden açılır ve `localhost:5000/products` API'sine bağlanır.

---

## 🔗 API Endpoint'leri

- `GET /products`: Tüm ürünleri getirir
- `POST /product`: Yeni ürün ekler  
  Body örneği:

```json
{
  "title": "Kalem",
  "price": 5.5
}
```

---

## 🎯 Arayüz Özellikleri

- Ürün listesi başlangıçta otomatik olarak sunucudan çekilir
- Yeni ürün formu ile ürün adı ve fiyat girilebilir
- Başarısız girişlerde kullanıcıya hata mesajı verilir
- React bileşen yapısı kullanılmıştır (`Header`, `NewProduct`, `ProductList`)

---
