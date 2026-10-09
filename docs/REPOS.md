# Abdullohkhan akkaunti — repolar xaritasi

Tekshirilgan sana: 2026-10-09. Har bir repo klon qilinib, ichi ochib ko'rildi:
README, package.json, `src/` tarkibi, commitlar tarixi, branchlar.

Jami: **30 repo** — 26 public + 4 private.
- 7 tasi **bo'sh** (birorta ham commit yo'q)
- 3 tasi **fork** (ichida sizning commitingiz yo'q)
- 2 tasi **archived**
- 1 tasi — shu profil repo (`Abdullohkhan`), hub hujjatlari shu yerda

> ⚠️ Asosiy akkaunt (Abdulmajidkhan007) hali tekshirilmadi — bu sessiyada
> unga kirish yo'q. "U yerda bormi?" ustuni keyingi qadamda to'ldiriladi.

---

## 🔴 Darhol qilinadigan ishlar (xavfsizlik)

Ikkita public repoda **maxfiy kalitlar** ochiq turibdi. Reponi o'chirish
yetarli emas — kalitlar allaqachon ko'chirib olingan bo'lishi mumkin.

1. **atoyo-new** → `src/integrations/telegram/index.ts` ichida **Telegram bot
   token** yozilgan (commit `80c4934`). BotFather → `/revoke` qilib yangi
   token oling. Yangi tokenni faqat `.env` ga yozing.
2. **Web11React** → `.env` fayli repoga tushgan: **SMTP login va parol**.
   Pochta parolini (yoki app-password) darhol almashtiring.
3. **atoyo-new** → `src/firebase/config.ts` da Firebase config bor. Bu
   o'zi sir emas, lekin Firestore/Storage **rules** to'g'ri yozilganini
   tekshiring (aks holda bazani har kim o'qiydi/yozadi).

Ko'chirishda bu fayllar tarix bilan birga ketmasligi kerak (pastga qarang).

---

## Qisqa jadval

| Repo | Holat | Taklif |
|---|---|---|
| atoyo-new | ✅ Eng to'liq loyiha | **Ko'chirish** (tarixsiz) |
| Atoyo-erp-v2 | 🟡 Katta, ishlaydi | **Ko'chirish** |
| Organick_org | ✅ Tugagan, deploy qilingan | **Ko'chirish** |
| portfolio-demo-2 | ✅ Tugagan | **Ko'chirish** |
| portfolio | ✅ Tugagan | Ko'chirish (yoki demo-2 bilan bitta) |
| memory-game | 🟡 Kichik, ishlaydi | Ixtiyoriy |
| 🔒 Atoyo | 🟡 Next.js do'kon, chala | Kerak emas (atoyo-new bor) |
| 🔒 desktop-tutorial | 🟡 Next.js dashboard + JWT reja | Ixtiyoriy |
| 🔒 nextjs | ⚪ Faqat shablon | Kerak emas |
| 🔒 tgbot | ⬜ Bo'sh | O'chirish |
| erp-system | ⚪ Faqat shablon | Kerak emas |
| atoyo-demo | ⚪ Faqat shablon | Kerak emas |
| portfolio-1 | 🔁 `portfolio` ning eski nusxasi | Kerak emas |
| portfolio-demo-1 | 🔁 `portfolio-demo-2` bilan bir xil | Kerak emas |
| Web11React | ⚠️ Archived, sir bor | Ko'chirmaslik |
| ojjo_project | 📚 O'quv (HTML/SCSS) | Ixtiyoriy |
| Web-6-Fronted | 🔁 `ojjo_project` nusxasi | Kerak emas |
| Creative_Studio_project | 📚 O'quv (HTML/CSS) | Ixtiyoriy |
| brArchitects | 📚 O'quv (HTML/CSS) | Ixtiyoriy |
| frap | 📚 O'quv (HTML/CSS) | Ixtiyoriy |
| AbdulmajidSharipov | ⬜ Bo'sh | O'chirish |
| Atoyo-erp | ⬜ Bo'sh | O'chirish |
| Atoyo-pro | ⬜ Bo'sh | O'chirish |
| BIOSWT | ⬜ Bo'sh (archived) | O'chirish |
| chat | ⬜ Bo'sh | O'chirish |
| portfolio-builder | ⬜ Bo'sh | O'chirish |
| DNS-over-Discord | 🍴 Fork | Kerak emas |
| realtime-chat-supabase-react | 🍴 Fork | Kerak emas |
| jack-portfolio | 🍴 Fork | Kerak emas |
| Abdullohkhan | 📄 Profil README + hub hujjatlari | Hujjatlar oxirida ko'chiriladi |

Belgilar: ✅ tugagan · 🟡 chala · ⚪ boshlanmagan · 🔁 dublikat ·
📚 o'quv mashqi · ⬜ bo'sh · 🍴 fork · ⚠️ muammo bor · 🔒 private

---

## Batafsil

### ✅ atoyo-new — ATOYO santexnika e-commerce
- **Nima:** Premium santexnika do'koni. Do'kon, savat, wishlist, checkout,
  login/register, user va admin dashboard (7 sahifa), blog, FAQ, yetkazib
  berish, kafolat sahifalari. Firebase (Auth, Firestore, Storage), Telegram
  bot orqali buyurtma xabari, Google Maps.
- **Stack:** React 19, TypeScript, Vite, Tailwind v4, MUI, Redux Toolkit,
  React Router v7, react-hook-form + zod, Framer Motion, Swiper.
- **Commitlar:** 6 ta, 2026-05-17 → 2026-05-18. Oxirgisi: "README.md
  loyiha haqida to'liq ma'lumot bilan yangilandi".
- **Diqqat:** Yagona branch — `claude/add-claude-documentation-cp7B1`
  (master yo'q). Bot token kodda (yuqoriga qarang).
- **Chala joylar:** OTP register olib tashlangan; admin sozlamalarida token
  inputlari bor, lekin env ishlatiladi. Production'ga chiqmagan ko'rinadi.
- **Taklif:** Ko'chirish — **tarixsiz** (yangi repo, bitta toza commit),
  token `.env` ga olinadi. Tugatish uchun alohida sessiya.

### 🟡 Atoyo-erp-v2 — Atoyo ERP (1C uslubida)
- **Nima:** Korxona uchun ERP: mijozlar, xodimlar, mahsulotlar,
  yetkazib beruvchilar, omborlar; sotuv (buyurtma, hisob-faktura),
  xarid (buyurtma, kirim), to'lovlar, hisobotlar (sotuv, qoldiq),
  dashboard (KPI, grafik). 62 ta `src` fayl.
- **Backend:** yo'q — `json-server` + `db.json` (soxta ma'lumot).
- **Stack:** React, TypeScript, Vite, MUI, Tailwind, Redux Toolkit,
  react-hook-form + zod, Recharts, xlsx (Excel eksport).
- **Commitlar:** 2 ta, 2026-05-08. Oxirgisi: "rename email".
- **Taklif:** Ko'chirish. Bo'sh `Atoyo-erp` va shablon `erp-system` shu
  loyihaning eski urinishlari — ular kerak emas.

### ✅ Organick_org — Organick (organik mahsulotlar do'koni)
- **Nima:** Ko'p sahifali sayt: bosh sahifa, haqida, do'kon + mahsulot
  sahifasi, blog, portfolio, xizmatlar, jamoa, aloqa formasi, 404.
- **Deploy:** https://organickorg.netlify.app/ (portfolio README'da).
- **Stack:** React, Vite, Tailwind v4, Redux Toolkit, React Router, motion.
- **Commitlar:** 3 ta, 2025-11-15. Oxirgisi: "del".
- **Chala joy:** README — standart Vite shabloni, almashtirish kerak.
- **Taklif:** Ko'chirish (portfoliodagi loyiha).

### ✅ portfolio-demo-2 — React portfolio (Dark/Light)
- **Nima:** Hero, About, Skills, Services, Portfolio, Testimonials,
  Contact, Footer; mavzu almashtirish, scroll-spy.
- **Stack:** React 19, TypeScript, Vite, Tailwind v4, MUI, Redux Toolkit.
- **Commitlar:** 2 ta, oxirgisi 2026-05-27.
- **portfolio-demo-1** bilan `src/` **100% bir xil**; demo-1 da qo'shimcha
  pnpm fayllari bor, xolos.
- **Taklif:** Ko'chirish (demo-2 ni). demo-1 kerak emas.

### ✅ portfolio — Bootstrap portfolio
- **Nima:** Vite + Bootstrap + SCSS shablon asosidagi portfolio
  (typed.js, AOS, Swiper, Isotope, Glightbox). README'da loyihalar ro'yxati
  (3D sayt, Organick va boshqalar).
- **Commitlar:** 3 ta, 2026-06-03 → 2026-06-04 (akkauntdagi eng oxirgi
  ish). Oxirgisi: "edit projects".
- **portfolio-1:** xuddi shu loyiha, 4 kun oldingi versiya (faqat
  `index.html`, `script.js`, `styles.scss` farq qiladi).
- **Taklif:** Bitta portfolio kifoya — qaysi biri asosiy ekanini siz
  hal qilasiz (Q1).

### 🟡 memory-game — Telegram Mini App xotira o'yini
- **Nima:** Karta juftlarini topish o'yini, `@telegram-apps/sdk`
  bilan. Butun mantiq bitta `App.jsx` da (160 qator).
- **Commitlar:** 2 ta, 2026-03-15.
- **Taklif:** Ixtiyoriy — kichik, lekin ishlaydigan.

### 🔒 Atoyo (private) — Atoyo'ning Next.js versiyasi
- **Nima:** Next.js (App Router) do'kon: home, shop + mahsulot sahifasi,
  login, dashboard, about, contact; Redux (auth, products, user);
  `api/upload` (Vercel Blob) — butunlay izohga olingan.
- **Commitlar:** 5 ta, 2026-02-28 → 2026-03-12. Oxirgisi: "edited".
- **Chala joylar:** README — standart create-next-app; upload ishlamaydi.
- **Taklif:** Kerak emas — atoyo-new (Vite) undan ancha to'liq. Faqat
  agar Atoyo'ni Next.js'da davom ettirish rejasi bo'lsa saqlanadi (Q5).

### 🔒 desktop-tutorial (private) — Next.js dashboard + auth mashqi
- **Nima:** Nomi aldaydi. `master` da Next.js dashboard (Sidebar, Navbar,
  StatsGrid, OverviewPanels — 9 komponent), `bcryptjs` + `jsonwebtoken`
  o'rnatilgan. `guide.txt` — register/login API va JWT middleware
  rejasi (hali yozilmagan). `me.md` — GitHub profil README qoralamasi
  ("Hi, I'm Abdulmajid", abdulmajid-sharipov.vercel.app). `branch2` —
  GitHub Desktop'ning asl tutorial commiti (2025-02-02).
- **Commitlar:** 2026-03-21 → 2026-03-23. Oxirgisi: "newuploaded".
- **Taklif:** Ixtiyoriy (Q5). `me.md` dagi stats rasmlari boshqa
  odamning (`abdujalil-nizomiddinov`) username'iga ulangan — ko'chirsa
  tuzatish kerak.

### 🔒 nextjs (private)
- create-next-app shabloni, 1 commit (2026-02-02). Taklif: kerak emas.

### 🔒 tgbot (private)
- Bo'sh, commit yo'q (2026-03-09 ochilgan). Taklif: o'chirish.

### ⚪ erp-system
- **Nima:** `master` — Vite shabloni (`App.tsx` 5 qator). `mobile`
  branch — Expo (React Native) shabloni. Firebase o'rnatilgan, kod yo'q.
- **Commitlar:** 1 ta, 2026-04-17.
- **Taklif:** Kerak emas (Atoyo-erp-v2 o'rnini bosadi).

### ⚪ atoyo-demo
- **Nima:** Vite shabloni + 34 qatorli `TestUI.tsx` (MUI sinovi).
- **Commitlar:** 1 ta, 2026-05-06.
- **Taklif:** Kerak emas (atoyo-new o'rnini bosadi).

### ⚠️ Web11React (archived)
- **Nima:** Nomi "React", aslida Express server: email orqali OTP
  yuborish (nodemailer). `node_modules` (703 fayl) va `.env` repoga
  tushib qolgan.
- **Commitlar:** 1 ta, 2025-10-23.
- **Taklif:** Ko'chirmaslik. Avval SMTP parolini almashtirish.

### 📚 O'quv mashqlari (HTML/CSS)
| Repo | Nima | Commit | Oxirgi |
|---|---|---|---|
| ojjo_project | OJJO zargarlik maketi (SCSS), Munisa bilan | 5 | 2025-01-17 |
| Web-6-Fronted | ojjo_project nusxasi (35 fayl bir xil) | 1 | 2025-01-20 |
| Creative_Studio_project | Creative Studio landing | 1 | 2025-06-04 |
| brArchitects | Arxitektura landing (`branch2`) | 3 | 2025-04-13 |
| frap | Bitta sahifa (index + rasm) | 2 | 2025-01-26 |

Taklif: agar asosiy akkauntda o'quv ishlar arxivi kerak bo'lsa —
`ojjo_project` ni ko'chirish yetarli, qolganlari ixtiyoriy (Q2).

### ⬜ Bo'sh repolar
`AbdulmajidSharipov`, `Atoyo-erp`, `Atoyo-pro`, `BIOSWT` (archived),
`chat`, `portfolio-builder`, `tgbot` (private) — hech qanday commit yo'q. Ko'chiradigan narsa
yo'q, akkaunt bilan birga o'chadi.

### 🍴 Forklar
`DNS-over-Discord` (MattIPv4), `realtime-chat-supabase-react`
(Shimon Wosner), `jack-portfolio` (Sadee) — ichida sizning birorta ham
commitingiz yo'q. Kerak bo'lsa, asosiy akkauntdan qayta fork qilinadi.

---

## Savollar (siz hal qilasiz)

- **Q1.** Portfolio: `portfolio` (Bootstrap) yoki `portfolio-demo-2`
  (React + TS) — qaysi biri asosiy? Ikkalasini ham ko'chiraymi?
- **Q2.** O'quv mashqlari (ojjo, Creative Studio, brArchitects, frap)
  kerakmi?
- **Q3.** memory-game ko'chirilsinmi?
- **Q4.** Abdulmajidkhan007 dagi repolar ro'yxatini bering (yoki o'sha
  akkauntni sessiyaga ulang) — dublikatlarni solishtirish uchun.
- **Q5.** Private repolardan `Atoyo` (Next.js) yoki `desktop-tutorial`
  (dashboard + JWT) ko'chirilsinmi?

## Keyingi qadamlar

1. Telegram token va SMTP parolini almashtirish (siz, telefondan).
2. Q1–Q5 javoblari → `docs/DECISIONS.md`.
3. Ko'chirish ro'yxati tasdiqlangach — har loyiha uchun alohida sessiya
   prompti (`docs/prompts/`).
