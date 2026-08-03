curl -i -X POST https://masar-class-api.a-f-almatrafi.workers.dev/api/posts \
 -H "Content-Type: application/json" \
 -d '{"title": "استكشاف", "body": "دورة كاملة", "author": "yourname"}'

curl -i https://masar-class-api.a-f-almatrafi.workers.dev/api/posts/ID

curl -i -X PATCH https://masar-class-api.a-f-almatrafi.workers.dev/api/posts/ID \
 -H "Content-Type: application/json" \
 -d '{"title": "استكشاف — معدَّل"}'

curl -i -X DELETE https://masar-class-api.a-f-almatrafi.workers.dev/api/posts/ID

curl -i https://masar-class-api.a-f-almatrafi.workers.dev/api/posts/ID
