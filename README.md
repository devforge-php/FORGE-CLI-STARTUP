Zo‘r tushundim. Quyida seni “**Forge**” loyihang uchun **to‘liq startup hujjati (docs)** shaklida mazmunli va aniq tarzda yozdim. Bu versiyani istalgan pitch, grant, yoki MVP-sahifada bemalol ishlatishing mumkin. 👇

---

# 🧱 **Forge – VPS boshqaruvini avtomatlashtiruvchi CLI vosita**

---

## 🚀 Startup maqsadi

**Forge** – bu dasturchilar va jamoalar uchun mo‘ljallangan, VPS serverlarni oddiy buyruqlar orqali yaratish, sozlash va boshqarishga yordam beradigan **CLI vosita**. Laravel Zero asosida ishlaydi.

---

## 🎯 Nima uchun kerak?

### 🧩 Muammo:

* Junior dasturchilar yoki kichik startup jamoalari ko‘pincha serverni sozlashda ko‘plab **xatoliklar qiladi**.
* Har safar yangi loyiha yoki branch uchun serverni **qo‘lda sozlash vaqt va resurslarni oladi**.
* Rollback (orqaga qaytish) va branch asosida serverni boshqarish **qo‘lda mushkul**.

### ✅ Yechim:

**Forge** yordamida:

* Bir necha **buyruq orqali** server yaratiladi va sozlanadi
* Har bir **branch alohida izolyatsiyalangan muhit** sifatida ishlaydi
* O‘zgarishlar **loglanadi va rollback qilish** mumkin bo‘ladi

---

## 👥 Kimlar uchun?

| Kim?                   | Qanday yordam beradi?                                                                    |
| ---------------------- | ---------------------------------------------------------------------------------------- |
| 👶 Junior dasturchilar | Serverni “plug-and-play” usulida o‘rganadi, real ish muhitida tajriba orttiradi          |
| 🚀 Startup jamoalari   | Tez prototiplash, testing branch’lari, CI/CD sodda tizimi                                |
| 🏢 Katta kompaniyalar  | Ko‘p sonli branch/serverlarni avtomatlashtirib, xavfsiz sozlash va boshqarish imkoniyati |

---

## 🧠 Asosiy funksiyalar (rejalashtirilgan)

| Buyruq                      | Tavsifi                                                               |
| --------------------------- | --------------------------------------------------------------------- |
| `forge init`                | Loyihani boshlaydi, kerakli papkalar va konfiguratsiyalarni yaratadi  |
| `forge connect <ip> <user>` | VPS serverga SSH orqali ulanadi va kerakli dasturlarni o‘rnatadi      |
| `forge branch <name>`       | Alohida branch yaratadi, har biri alohida konfiguratsiyani ifodalaydi |
| `forge deploy`              | Joriy branchdagi sozlamalarni serverga o‘rnatadi                      |
| `forge commit "<msg>"`      | O‘zgarishlarni snapshot sifatida saqlaydi (config-as-code)            |
| `forge rollback`            | Oldingi holatga qaytaradi                                             |
| `forge delete <name>`       | Branchni o‘chiradi va kerakli tozalash ishlarini amalga oshiradi      |
| `forge main merge <name>`   | `<name>` branchdagi sozlamalarni asosiy `main` branchga birlashtiradi |
| `forge list`                | Barcha branch va ularning holatini ko‘rsatadi                         |

---

## 🔐 Xavfsizlik

* SSH orqali ulanishda maxsus autentifikatsiya tekshiruvi
* Har bir branchda rollback log saqlanadi
* `main` branch faqat tasdiqlangan o‘zgarishlar bilan yangilanadi

---

## 🔮 Kelajakdagi imkoniyatlar (Post-MVP)

* GUI interfeys (web yoki desktop) orqali CLI'ni boshqarish
* GitHub bilan integratsiya (CI/CD uchun)
* Laravel Forge, DigitalOcean API, Hetzner API bilan avtomatik server yaratish
* `.forge.yml` orqali sozlamalarni avtomatik yangilash

---

## 📌 Umumiy xulosa

**Forge** — bu `git` falsafasiga o‘xshash tarzda VPS’larni boshqarish imkonini beruvchi, soddalashtirilgan, kuchli va xavfsiz CLI vositasi. Laravel asosida qurilishi orqali PHP dunyosidagi dasturchilar uchun kirish oson, ishlab chiqish qulay bo‘ladi.

---

Agar xohlasang, bu hujjatni PDF, Word yoki `README.md` shaklida qilib beraman. Qanday formatda kerak?
