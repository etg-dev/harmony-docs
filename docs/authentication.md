# احراز هویت با OAuth 2.0

Harmony از استاندارد OAuth 2.0 (Authorization Code Flow) برای احراز هویت استفاده می‌کند.

## مراحل احراز هویت

۱. هدایت کاربر به:

```
GET https://sheypoor.com/oauth/authorize
```

۲. دریافت `authorization_code` از طریق `redirect_uri`.

۳. ارسال کد به آدرس توکن:

```
POST https://sheypoor.com/oauth/token
```

پاسخ:

```json
{
  "access_token": "توکن دسترسی",
  "token_type": "bearer",
  "expires_in": 3600,
  "refresh_token": "توکن رفرش"
}
```
