# توثيق دورة CRUD الكاملة

تمت تجربة الأوامر بنجاح وتوثيق الاستجابات (Status Codes) الفعلية لكل خطوة كما يلي:

## 1. إنشاء منشور جديد (POST)
- **الأمر المُنفذ:**
```bash
curl -i -X POST https://masar-class-api.a-f-almatrafi.workers.dev/api/posts \
  -H "Content-Type: application/json" \
  -d '{"title": "استكشاف", "body": "دورة كاملة", "author": "اسمك"}'
```
- **رمز الحالة (Status Code):** `201 Created`

## 2. قراءة المنشور (GET)
- **الأمر المُنفذ:**
```bash
curl -i https://workers.dev
```
- **رمز الحالة (Status Code):** `200 OK`

## 3. تعديل المنشور (PATCH)
- **الأمر المُنفذ:**
```bash
curl -i -X PATCH https://workers.dev \
  -H "Content-Type: application/json" \
  -d '{"title": "استكشاف - معدل"}'
```
- **رمز الحالة (Status Code):** `200 OK`

## 4. حذف المنشور (DELETE)
- **الأمر المُنفذ:**
```bash
curl -i -X DELETE https://workers.dev
```
- **رمز الحالة (Status Code):** `200 OK`

## 5. التحقق من الحذف (GET للتحقق)
- **الأمر المُنفذ:**
```bash
curl -i https://workers.dev
```
- **رمز الحالة (Status Code):** `404 Not Found`
