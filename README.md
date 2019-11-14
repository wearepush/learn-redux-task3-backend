# Backend для тестового задания #3

### Поддерживаемые маршруты:

```js
// Корневой адрес API: http://localhost:8080/api/v1

// POST /validate (введены корректные данные: email = 'admin@test.com', password = '12345'
{
  "status": "ok",
  "data": {
    "id": 1
  }
}

// POST /validate (введены некорректные данные)
{
  "status": "err",
  "message": "wrong_email_or_password"
}

// GET /user-info/:id - где, id - идентификатор пользователя
// GET /user-info/1
{
  "status": "ok",
  "data": {
    "id": 1,
  }
}

// GET /user-info/2
{
  "status": "err",
  "message": "user_not_found"
}

// GET /news
{
  "status": "ok",
  "data": [
  ]
}
```

### Запуск

```sh
# Install dependencies
npm install

# Start development live-reload server
npm run dev

# Start production server:
npm start
```
