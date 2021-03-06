# E-commerce Tracking with Google Analytics Tag

### 8 steps of e-commerce ###
- Home
- Category
- Product
- Add Cart / Remove Cart
- Checkout
- Shipping
- Payment
- Thanks

#### Home
View internal promotion banner แสดงแบนเนอร์โปรโมชั่นบนหน้าเว็บ<br>
**- เก็บค่าการแสดงผลของแต่ละแบนเนอร์ ที่ตำแหน่งต่างๆ**

#### Category
Click on promotion banner and view products in product list คลิกที่แบนเนอร์โปรโมชั่นจากหน้า *Home* แล้วมาแสดงผลรายการสินค้าที่หน้า *Category*<br>
**- เก็บว่าคลิกที่แบนเนอร์ไหนมา**<br>
**- เก็บค่าการแสดงรายการสินค้า และตำแหน่งของสินค้าในรายการนั้นๆ**

#### Product
Click on product in product list and and view product detail คลิกที่สินค้าจากหน้า *Category* แล้วมาหน้าแสดงรายละเอียดสินค้าของนั้นๆ<br>
**- เก็บว่าคลิกที่รายการสินค้าตำแหน่งไหนมา**<br>
**- เก็บค่าการแสดงผลหน้ารายละเอียดสินค้า**

#### Add Cart / Remove Cart
Add product to shopping cart คลิกเพิ่มสินค้าไปที่ตระกร้าสินค้า<br>
**- เก็บว่าคลิกสินค้าไหนเข้าตระกร้าบ้าง**

Remove product form shopping cart คลิกลบสินค้าออกจากตระกร้าสินค้า<br>
**- เก็บว่าคลิกสินค้าไหนออกจากตระกร้าบ้าง**

__BUG__ : ถ้าใช้ <a href="https://developers.google.com/analytics/devguides/collection/gtagjs/">gtag.js</a> ค่า Product List Name ไม่แสดง จะขึ้นเป็น (not set)
แก้โดยกลับไปใช้ <a href="https://developers.google.com/analytics/devguides/collection/analyticsjs/">analytics.js</a> แทน

#### Checkout
Begin checkout step ส่งค่ารายละเอียดสินค้าจากตระกร้าเข้าสู่กระบวนการ checkout ใส่คูปองไปก็เท่านั้น ค่าไม่ขึ้น เพราะจะเก็บค่าได้ตอน event purchase เท่านั้น<br>
**- เก็บว่าซื้อสินค้าอะไรบ้าง**<br>
**- เก็บว่า option ของ step นี้**

__BUG__ : ถ้าใช้ <a href="https://developers.google.com/analytics/devguides/collection/gtagjs/">gtag.js</a> ค่า Product List Name ไม่แสดง จะขึ้นเป็น (not set)
แก้โดยกลับไปใช้ <a href="https://developers.google.com/analytics/devguides/collection/analyticsjs/">analytics.js</a> แทน

#### Shipping
Shipping checkout step ส่งค่ารายละเอียดสินค้า และค่า option ว่าจัดส่งยังไง<br>
**- เก็บว่าผ่านมา step นี้ไหม**<br>
**- เก็บค่า option ของ step นี้**

#### Payment
Payment checkout step ส่งค่ารายละเอียดสินค้า และค่า option ว่าจ่ายเงินยังไง<br>
**- เก็บว่าผ่านมา step นี้ไหม**<br>
**- เก็บค่า option ของ step นี้**

#### Thanks
Purchase complete with transaction ส่งค่า transaction รายละเอียดสินค้า รวมถึงคูปองที่ใช้ทั้งหมด<br>
**- เก็บค่าสินค้าที่ซื้อ**<br>
**- เก็บราคา ภาษี ค่าขนส่ง**<br>
**- เก็บว่าใช้คูปองอะไรบ้าง**<br>
**- เก็บว่าซื้อผ่าน affiliate อะไร**

---

Favicon made by <a href="https://www.flaticon.com/authors/bqlqn" title="bqlqn">bqlqn</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
is licensed by <a href="http://creativecommons.org/licenses/by/3.0/" title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a>
