REST API
запрос

GET /api/v1/partner-shops HTTP/1.1
Host: api.petrushka-green.ru
Accept: application/json

пример ответа

{
  "success": true,
  "data": [
    {
      "id": 1,
      "name": "ВкусВилл",
      "description": "Натуральные продукты и готовая еда",
      "logoUrl": "https://cdn.petrushka-green.ru/partners/vkusvill.png",
      "bannerUrl": "https://cdn.petrushka-green.ru/partners/vkusvill-banner.jpg",
      "link": "https://vkusvill.ru",
      "backgroundColor": "#4CAF50"
    },
    {
      "id": 2,
      "name": "Самокат",
      "description": "Быстрая доставка продуктов",
      "logoUrl": "https://cdn.petrushka-green.ru/partners/samokat.png",
      "bannerUrl": "https://cdn.petrushka-green.ru/partners/samokat-banner.jpg",
      "link": "https://samokat.ru",
      "backgroundColor": "#FF69B4"
    },
    {
      "id": 3,
      "name": "Яндекс Лавка",
      "description": "Доставка продуктов за 15 минут",
      "logoUrl": "https://cdn.petrushka-green.ru/partners/lavka.png",
      "bannerUrl": "https://cdn.petrushka-green.ru/partners/lavka-banner.jpg",
      "link": "https://lavka.yandex.ru",
      "backgroundColor": "#FFD400"
    }
  ]
}

возможный ответ при отсутствии партнёров

{
  "success": true,
  "data": []
}

возможный ответ при ошибке

{
  "success": false,
  "error": {
    "code": "INTERNAL_ERROR",
    "message": "Не удалось загрузить список партнеров."
  }
}