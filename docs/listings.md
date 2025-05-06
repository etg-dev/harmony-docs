# API لیستینگ

## دریافت لیست آگهی‌ها

```
GET /api/listings
Authorization: Bearer {access_token}
```

### پاسخ:

```json
[
  {
    "id": 123,
    "title": "فروش آپارتمان ۸۰ متری",
    "price": 2500000000,
    "location": "تهران، سعادت‌آباد"
  }
]
```

## ایجاد آگهی جدید

```
POST /api/listings
Authorization: Bearer {access_token}
Content-Type: application/json
```

```json
{
  "title": "فروش لپ‌تاپ",
  "description": "لپ‌تاپ در حد نو، مدل XYZ",
  "price": 15000000,
  "category": "الکترونیک",
  "location": "تهران، ونک"
}
```
