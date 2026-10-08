const basePrice = bookingReservation.priceKey
priceKey đang có giá trị là const priceKey = "roomPrice";
Khi viết bookingReservation.priceKey
-> Bị hiểu là tìm thuộc tính có tên priceKey trong object
Nhưng obj kh có thuộc tính priceKey mà chỉ có roomPrice: 1500000 vì thế nên bookingReservation.priceKey -> underfined

Sửa: const basePrice = bookingReservation[priceKey];