
# Stripe Checkout Server (Express + Render)

## 📦 Установка

```bash
npm install
```

## 🚀 Запуск локально

Создай `.env` файл:

```
STRIPE_SECRET_KEY=sk_test_...
```

```bash
node server.js
```

## 🌐 Развёртывание на Render

1. Подключи GitHub репозиторий
2. Создай Web Service:
   - Build Command: `npm install`
   - Start Command: `npm start`
3. Установи переменную среды `STRIPE_SECRET_KEY`
4. Готово ✅

## 🧪 Тест запроса

```http
POST /create-checkout-session
Content-Type: application/json

{
  "items": [
    {
      "price": "price_XXX",
      "quantity": 1
    }
  ]
}
```
