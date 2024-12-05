# সিলেটী দোকান 🛍️
- [Software Requirements Specification](README.md)
- [REST API Endpoints](REST-API-Design.md)

## API Endpoints 🧩

### User  
- POST - /api/v1/user/new
- GET - /api/v1/user/all ✨ Admin
- GET - /api/v1/user/:id
- DELETE - /api/v1/user/:id ✨ Admin

### Product
- POST - /api/v1/product/new ✨ Admin
- GET - /api/v1/product/latest
- GET - /api/v1/product/all
- GET - /api/v1/product/categories
- GET - /api/v1/product/admin-product ✨ Admin
- GET - /api/v1/product/:id ✨ Admin
- PUT - /api/v1/product/:id ✨ Admin
- DELETE - /api/v1/product/:id ✨ Admin

### Order
- POST - /api/v1/order/new
- GET - /api/v1/order/my
- GET - /api/v1/order/all ✨ Admin 
- GET -  /api/v1/order/:id
- PUT -  /api/v1/order/:id
- DELETE - /api/v1/order/:id

### Payment
- POST - /api/v1/payment/create
- POST - /api/v1/payment/coupon/new ✨ Admin
- GET - /api/v1/payment/discount/apply
- GET - /api/v1/payment/coupon/all ✨ Admin
- DELETE - /api/v1/payment/coupon/:id ✨ Admin

### Admin Dashboard
- GET - /api/v1/admin/dashboard/stats
- GET - /api/v1/admin/dashboard/pie
- GET - /api/v1/admin/dashboard/bar
- GET - /api/v1/admin/dashboard/line

