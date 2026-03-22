# 🕹️ ARCADE VAULT — منصة سحابية تلقائية

> **الموقع يكتشف ألعابك تلقائياً من مجلد `roms/` — بدون أي إعداد يدوي**

---

## 📁 هيكل المشروع

```
arcade-vault/
├── index.html     ← الموقع الكامل (لا تعدّل عليه)
├── roms/          ← 📦 فقط ضع ملفات الروم هنا
│   ├── sonic.md
│   ├── mario.nes
│   └── zelda.gba
├── .nojekyll
└── README.md
```

---

## ⚡ إضافة لعبة — خطوة واحدة فقط

```bash
# ضع الملف في مجلد roms/ وارفعه
git add roms/sonic.md
git commit -m "add Sonic"
git push
# ✅ اللعبة تظهر تلقائياً!
```

**الموقع يكتشف تلقائياً:**
- 📛 اسم اللعبة من اسم الملف
- 🎮 النظام من امتداد الملف (.nes → NES, .gba → GBA...)
- 🖼️ الغلاف من Libretro Thumbnails

---

## 🎮 الامتدادات المدعومة

| الامتداد | النظام |
|----------|--------|
| `.nes` | Nintendo NES |
| `.smc` `.sfc` | Super Nintendo |
| `.n64` `.z64` | Nintendo 64 |
| `.gb` | Game Boy |
| `.gbc` | Game Boy Color |
| `.gba` | Game Boy Advance |
| `.nds` | Nintendo DS |
| `.md` `.gen` | Sega Mega Drive |
| `.sms` | Sega Master System |
| `.gg` | Sega Game Gear |
| `.bin` `.pbp` | PlayStation 1 |
| `.iso` `.cso` | PSP |
| `.zip` | Arcade (FBNeo/MAME) |
| `.a26` | Atari 2600 |

---

## ⚙️ الإعدادات (في الموقع)

اضغط **⚙** في أعلى الصفحة للوصول إلى:

- **GitHub Repository** — إذا لم يُكتشف تلقائياً
- **Core Selector** — اختر Core محاكاة لكل نظام  
- **BIOS URLs** — لأنظمة تحتاج BIOS (PS1، Sega CD...)
- **CRT Shaders** — فلاتر بصرية (Scanlines، CRT، Neon...)
- **CORS Proxy** — لحل مشاكل الروابط الخارجية
- **Box Art** — تفعيل/إيقاف أغلفة الألعاب الحقيقية

---

## 🌐 رفع على GitHub Pages

1. **New Repository** → `arcade-vault` → **Public**
2. ارفع `index.html` + مجلد `roms/` + `.nojekyll`
3. **Settings** → **Pages** → **Branch: main** → **Save**
4. ✅ موقعك جاهز: `https://[username].github.io/arcade-vault/`

الموقع يكتشف تلقائياً أنه على GitHub Pages ويقرأ مجلد roms/ مباشرة!

---

**ARCADE VAULT · Auto-Scan · No Config Needed**
