# Forge

**CLI vositasi orqali VPS serverlarni avtomatik boshqarish**

---

## Nima uchun kerak & Nima qiladi?
- **Muammo:** Junior dasturchilar va kichik jamoalar VPS’ni qo‘lda sozlashda ko‘plab xatolarga yo‘l qo‘yadi, vaqt va resurs sarflanadi.  
- **Yechim:** Bir nechta buyruq bilan serverni yaratish, konfiguratsiya qilish, o‘zgartirishlarni saqlash va xatolarni rollback qilish imkoniyatini taqdim etadi.  

---

## Kimlar uchun foydali?
- **Junior dasturchilar:** Serverni o‘rnatish va sozlashni “plug‑and‑play” usulida o‘rganadi.  
- **Startup jamoalari:** Tez prototip yaratish va muhitni boshqarishni soddalashtiradi.  
- **Katta kompaniyalar:** Ko‘p sonli serverlarni branch‑asosida boshqarish va xavfsiz rollback qilish imkonini beradi.  

---

## Asosiy buyruqlar

| Buyruq                            | Nima qiladi                                              | Nega kerak?                                   |
|-----------------------------------|----------------------------------------------------------|-----------------------------------------------|
| `forge init`                     | Yangi VPS yaratadi va default paketlarni o‘rnatadi       | Tez va xatosiz birinchi sozlash               |
| `forge branch <name>`            | `<name>` nomli izolyatsiya qilingan branch yaratadi      | Eksperiment qilish uchun xavfsiz muhit         |
| `forge all`                      | Joriy branch uchun barcha konfiguratsiyalarni tatbiq etadi | Branch muhitini to‘liq ishga tushirish         |
| `forge commit "<msg>"`           | O‘zgarishlarni logga yozadi va snapshot yaratadi         | Qadam‑qadam o‘zgarishlarni kuzatish            |
| `forge delete <name>`            | `<name>` branchni o‘chiradi va rollback qiladi           | Xatolik bo‘lsa tozalash va yangidan boshlash   |
| `forge main merge <name>`        | `<name>` branchdagi tasdiqlangan o‘zgarishlarni main ga qo‘shadi | Ishchi konfiguratsiyani asosiyga ko‘tarish      |