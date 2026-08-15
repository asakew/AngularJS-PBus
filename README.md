# Proyekt: Avtobus Parkovka Menejeri (Bus Parking Manager)

Ushbu loyiha avtobuslar saroyidagi (parkovka) harakatni boshqarish va monitoring qilish uchun mo'ljallangan sodda ma'lumotlar bazasi tizimidir. Loyiha doirasida avtobuslarning yo'nalishlari, haydovchilar ma'lumotlari hamda parkovkaga kirish-chiqish vaqtlari hisobga olingan.

## Ma'lumotlar Bazasi Jadvali (Database Table)

Tizimning asosiy yadrosini quyidagi ustunlardan (fields) iborat jadval tashkil etadi:

| Ustun Nomi (Field) | Ma'lumot Turi (Data Type) | Tavsif (Description) |
| :--- | :--- | :--- |
| **Mashrut Num** | VARCHAR / INT | Avtobus qatnaydigan yo'nalish (marshrut) raqami |
| **Ism va Familiya** | VARCHAR | Avtobusni boshqarayotgan haydovchining to'liq ismi |
| **outTime** | DATETIME / TIME | Avtobusning parkovkadan chiqib ketgan vaqti |
| **inTime** | DATETIME / TIME | Avtobusning parkovkaga qaytib kirgan vaqti |

## Loyihaning Asosiy Funksiyalari

*   **Avtobuslar Monitoringi:** Qaysi marshrut tizimda faol ekanligini va qachon qaytganini kuzatish.
*   **Vaqt Nazorati:** `outTime` va `inTime` yordamida avtobuslarning chiziqdagi (reysdagi) umumiy vaqtini hisoblash.
*   **Haydovchilar Hisobi:** Har bir marshrutga biriktirilgan mas'ul xodimlarni boshqarish.

## Texnologiyalar

*   **Frontend:** AngularJS, HTML/CSS (interfeys uchun)
