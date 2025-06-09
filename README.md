
---

## ✅ Loyiha nomi (ishchi nom):

**Forge CLI** — Laravel serverlar uchun Git-falsafasiga asoslangan boshqaruv vositasi

---

## 🧑‍💻 Kimlar uchun:

* Laravel backend dasturchilar
* Laravel jamoalarda (team) ishlovchi developerlar
* VPS serverlarda ishlaydigan fullstacklar
* Laravel loyihasini deploy qilmoqchi bo‘lgan o‘quvchilar / juniorlar
* DevOps va Laravelni birlashtirmoqchi bo‘lgan kompaniyalar

---

## 🎯 Loyihaning asosiy maqsadi:

Laravel developerlar uchun **Docker’siz**, **bash’siz**, **manual konfiguratsiyasiz** tarzda VPS serverga Laravel loyihani o‘rnatish, boshqarish va rivojlantirishni **CLI buyruqlar** orqali soddalashtirish.

---

## ❌ Yechiladigan muammolar:

| Muammo                                                            | Yechim                                                                  |
| ----------------------------------------------------------------- | ----------------------------------------------------------------------- |
| VPS serverga Laravel loyihani qo‘lda o‘rnatish — uzoq va chalkash | `forge init` bilan Laravel + PHP + MySQL + Nginx avtomatik o‘rnatiladi  |
| Bir nechta dasturchi bir serverda ishlay olmaydi                  | Har bir dasturchiga `forge branch` orqali alohida muhit                 |
| Server konfiguratsiyasi noto‘g‘ri sozlansa rollback yo‘q          | `forge commit`, `forge rollback` bu muammoni hal qiladi                 |
| Docker o‘rganish majburiyligi                                     | Docker kerakmas, oddiy `.env`, `.conf` fayllar asosida                  |
| Dasturchi noto‘g‘ri konfiguratsiya qilsa hamma uchun buziladi     | Har bir branch izolyatsiyalangan — izolyatsiya Git falsafasiga o‘xshash |

---

## ⚙️ Asosiy funksiyalar rejasi:

### 🔧 `forge init`

> VPS serverda kerakli hamma narsani o‘rnatadi:

* PHP, MySQL/PostgreSQL, Composer, Nginx, Laravel
* Laravel loyihasi yaratadi yoki GitHub’dan klon qiladi
* `.env`, `nginx.conf` avtomatik yaratiladi

---

### 🌿 `forge branch <ism>`

> Har bir developer o‘ziga alohida test muhitini yaratadi

* Laravel loyihasi kloni yaratiladi
* Alohida `.env` fayl
* Alohida `nginx` port (masalan: `8001`, `8002`, ...)
* Branch katalog nomi: `forge_branch_ism`

---

### 💾 `forge commit`

> O‘z branch’ida qilgan ishlarni saqlaydi

* Konfiguratsiya, `.env`, nginx sozlamalarini snapshot qiladi
* Agar branch ishlamasa, `rollback` qilish mumkin

---

### 🔙 `forge rollback`

> So‘nggi `commit`ga qaytish

* Server konfiguratsiyasi, `.env` qayta tiklanadi

---

### 🔁 `forge merge <branch>`

> Branch ichidagi o‘zgarishlarni `main` muhitga qo‘shish

* Testdan o‘tgan so‘nggina merge bo‘ladi

---

### 🗑️ `forge destroy <branch>`

> Branch’ni o‘chiradi, agar kerak bo‘lmasa

---

### 📦 `forge deploy`

> Hozirgi holatni production VPS’ga deploy qiladi

---

### 🔐 `forge ssh`

> Branch ichiga terminal orqali kira olish

---

### ⚙️ `forge config:set <key> <value>`

> `.env` va `nginx.conf` sozlamalarini branch asosida o‘zgartirish

---

## 🧠 Yordamchi buyruqlar (keyinchalik qo‘shiladi):

* `forge list` — barcha branchlar ro‘yxati
* `forge status` — joriy branch holati
* `forge logs` — branch log fayllari
* `forge pull <repo>` — Laravel loyihani GitHub’dan olish
* `forge install <package>` — branch ichiga Laravel package o‘rnatish

---

## 📦 Texnologiyalar:

| Texnologiya          | Vazifasi                                           |
| -------------------- | -------------------------------------------------- |
| **Laravel Zero**     | CLI tuzish uchun framework                         |
| **PHP**              | CLI logika va Laravel integratsiya                 |
| **SSH**              | VPS ulanish va fayl uzatish                        |
| **Bash**             | Fayl va konfiguratsiya o‘zgarishlari               |
| **Nginx**            | Har bir branch uchun port orqali server sozlash    |
| **MySQL/PostgreSQL** | Ma’lumotlar bazasi (har branch uchun prefiksli DB) |

---

## 📄 GitHub README uchun tayyor matn (soddalashtirilgan):

```markdown
# Forge CLI 🔥

Laravel developerlar uchun VPS server boshqaruv vositasi. Har bir developer o‘z branch'ida mustaqil ishlaydi. Git falsafasiga o‘xshash CLI.

## 🔧 O‘rnatish
```

composer global require username/forge-cli

```

## ⚙️ Asosiy buyruqlar

| Buyruq | Maqsadi |
|--------|---------|
| `forge init` | Laravel serverni to‘liq sozlash |
| `forge branch ali` | `ali` ismli branch ochish |
| `forge commit` | Konfiguratsiyani saqlash |
| `forge rollback` | So‘nggi sozlamaga qaytish |
| `forge merge ali` | `ali` branch’ni asosiyga qo‘shish |
| `forge destroy ali` | Branch’ni o‘chirish |
| `forge deploy` | Productionga chiqarish |
| `forge ssh` | Branch terminaliga kirish |

## 🧠 Nega kerak?

- VPS'da tez Laravel deploy
- Har dasturchiga mustaqil muhit
- Rollback, commit, merge – Git falsafasida
- Docker'siz server boshqaruvi

## 🧱 Litsenziya
MIT License
```

---
