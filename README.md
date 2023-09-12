Получение информации о карточке товара с отзывами
Метод: GET
Путь: /api/product/{product_id}
Описание: Этот метод возвращает информацию о карточке товара вместе с отзывами, связанными с этим товаром.
Параметры запроса:
product_id (путь) - уникальный идентификатор товара.

{
  "product_info": {
    "product_id": "12345",
    "product_name": "Название товара",
    "product_description": "Описание товара",
    "product_price": 1999.99,
    "product_reviews": [
      {
        "review_id": "1",
        "user_name": "Пользователь 1",
        "rating": 4,
        "review_text": "Отличный товар!",
        "review_date": "2023-09-01",
        "review_images": [
          "url_to_image1.jpg",
          "url_to_image2.jpg"
        ]
      },
      {
        "review_id": "2",
        "user_name": "Пользователь 2",
        "rating": 5,
        "review_text": "Замечательный товар!",
        "review_date": "2023-09-02",
        "review_images": []
      }
    ]
  }
}
