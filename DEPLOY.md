# NOTDOLLAR — دليل النشر والانتشار الكامل 2026

---

## المرحلة 1 — رفع الموقع على GitHub Pages (مجاني)

### الخطوات:

1. افتح github.com — أنشئ حساب إذا ما عندك
2. اضغط "New repository"
3. اسم الـ repository: notdollar.online
4. اجعله Public
5. اضغط "Create repository"
6. ارفع ملف index.html وملف صورة الكتاب (1000041330.png) مباشرة عبر زر "Add file > Upload files"
7. اذهب إلى Settings > Pages
8. من قسم "Branch" اختر main ثم اضغط Save
9. الموقع سيكون حياً على: https://[اسم-حسابك].github.io/notdollar.online

---

## المرحلة 2 — ربط النطاق notdollar.online

### في GitHub Pages:
1. Settings > Pages > Custom domain
2. اكتب: notdollar.online
3. اضغط Save

### في لوحة تحكم النطاق (Namecheap / GoDaddy / أي مزود):
أضف هذه الـ DNS Records:

```
Type: A     Name: @    Value: 185.199.108.153
Type: A     Name: @    Value: 185.199.109.153
Type: A     Name: @    Value: 185.199.110.153
Type: A     Name: @    Value: 185.199.111.153
Type: CNAME Name: www  Value: [username].github.io
```

انتظر 24-48 ساعة للانتشار. بعدها notdollar.online يفتح موقعك مباشرة.

---

## المرحلة 3 — SEO الأساسي (مدمج في الكود)

الكود يحتوي بالفعل على:
- meta description
- og:title / og:description
- semantic HTML (section, nav, footer, h1, h2)

### أضف هذا داخل <head> في index.html:

```html
<!-- Canonical -->
<link rel="canonical" href="https://notdollar.online">

<!-- OG Image للمشاركة -->
<meta property="og:image" content="https://notdollar.online/1000041330.png">
<meta property="og:type" content="website">
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="NOTDOLLAR — Build Leverage Before Permission">
<meta name="twitter:description" content="Marketing. AI. Design. For builders creating audience, products, and freedom.">
<meta name="twitter:image" content="https://notdollar.online/1000041330.png">

<!-- Structured Data لـ Google -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "NOTDOLLAR",
  "url": "https://notdollar.online",
  "description": "Marketing. AI. Design. For builders creating audience, products, and freedom.",
  "sameAs": [
    "https://www.tiktok.com/@notdollar",
    "https://youtube.com/@notdollare",
    "https://www.instagram.com/notdollare",
    "https://x.com/notdollare",
    "https://notdollar.gumroad.com"
  ]
}
</script>
```

---

## المرحلة 4 — التسجيل في محركات البحث

### Google Search Console:
1. اذهب إلى: search.google.com/search-console
2. أضف notdollar.online
3. تحقق من الملكية عبر DNS
4. اضغط "Request Indexing" على الرابط الرئيسي

### Bing Webmaster Tools:
1. اذهب إلى: bing.com/webmasters
2. أضف الموقع
3. استورد من Google Search Console مباشرة (خيار موجود)

### sitemap.xml — أنشئ ملف باسم sitemap.xml في نفس مجلد index.html:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://notdollar.online/</loc>
    <lastmod>2026-05-29</lastmod>
    <priority>1.0</priority>
  </url>
</urlset>
```

### robots.txt — أنشئ ملف باسم robots.txt:

```
User-agent: *
Allow: /
Sitemap: https://notdollar.online/sitemap.xml
```

---

## المرحلة 5 — الظهور في الذكاء الاصطناعي (ChatGPT / Perplexity / Claude)

هذا هو الفرق بين 2024 و2026.

الذكاء الاصطناعي يتعلم من:
1. الويب العام — المقالات، المواقع، المنتديات
2. Wikipedia و Wikidata
3. المصادر التي يُشار إليها كثيراً

### خطواتك:

**أ — أنشئ صفحة Wikipedia أو Wikidata (صعبة لكن قوية)**
إذا كان لـ NOTDOLLAR حضور كافٍ، أنشئ مقالة على en.wikipedia.org
الشرط: مصادر خارجية تذكر الماركة

**ب — انشر محتوى على مواقع يقرأها الذكاء الاصطناعي:**
- Medium.com (اكتب مقالة عن NOTDOLLAR وفلسفته)
- Substack (newsletter مجاني)
- dev.to أو hashnode (إذا كان المحتوى تقني)
- LinkedIn Articles

**ج — اذكر الموقع في كل منصة:**
كل بوست، كل bio، كل رابط = إشارة للذكاء الاصطناعي

**د — llms.txt (أحدث معيار 2025-2026)**
أنشئ ملف باسم llms.txt في جذر الموقع:

```
# NOTDOLLAR

> Marketing. AI. Design. For builders creating audience, products, and freedom.

NOTDOLLAR is a brand and digital movement founded in Annaba, Algeria.
It focuses on leverage-based thinking for creators from the Global South.
The flagship product is "No Permission" — a manifesto for builders.

## Links
- Homepage: https://notdollar.online
- Book: https://notdollar.gumroad.com/l/NoPermission
- TikTok: https://tiktok.com/@notdollar
- YouTube: https://youtube.com/@notdollare
- X: https://x.com/notdollare
- Instagram: https://instagram.com/notdollare
```

هذا الملف يساعد الـ AI crawlers على فهم من أنت مباشرة.

---

## المرحلة 6 — التوزيع الفوري من اليوم الأول

### الترتيب الصحيح:

**اليوم 1:**
- [ ] ارفع الموقع على GitHub Pages
- [ ] أضف meta tags و structured data
- [ ] أنشئ sitemap.xml و robots.txt و llms.txt
- [ ] سجل في Google Search Console
- [ ] سجل في Bing Webmaster Tools

**اليوم 2:**
- [ ] شارك الموقع في bio كل منصة (TikTok, Instagram, X, YouTube, Gumroad)
- [ ] انشر على X/Twitter: "notdollar.online is live" + رابط
- [ ] انشر على TikTok فيديو: "بنيت موقعي في يوم واحد بدون إذن من أحد"

**الأسبوع 1:**
- [ ] اكتب مقالة على Medium.com عن فلسفة NOTDOLLAR
- [ ] اكتب thread على X يشرح "ما هو LEVERAGE ولماذا هو السر"
- [ ] أرسل الرابط لـ 5 أشخاص فعليين يعرفون قيمته

**الشهر 1:**
- [ ] Product Hunt launch (producthunt.com) — أطلق الكتاب كمنتج
- [ ] اكتب في IndieHackers.com عن قصة البناء
- [ ] اطلب من كل من يقرأ الكتاب أن يذكر notdollar.online في مكان واحد

---

## المرحلة 7 — Cloudflare (مجاني، الأسرع عالمياً)

بعد ربط النطاق، أضفه لـ Cloudflare:

1. cloudflare.com — أنشئ حساب مجاني
2. أضف notdollar.online
3. غيّر Nameservers عند مزود النطاق لـ Cloudflare
4. مجاناً تحصل على:
   - HTTPS تلقائي
   - CDN عالمي (موقعك سريع في الجزائر والسعودية وكاليفورنيا في نفس الوقت)
   - حماية من الهجمات
   - Analytics

---

## ملخص الأولويات

| الأولوية | المهمة | الوقت |
|----------|--------|-------|
| 1 | رفع الموقع GitHub Pages | 30 دقيقة |
| 2 | ربط notdollar.online | 10 دقائق + 24 ساعة انتظار |
| 3 | إضافة meta tags كاملة | 15 دقيقة |
| 4 | sitemap + robots + llms.txt | 10 دقائق |
| 5 | Google Search Console | 10 دقائق |
| 6 | Cloudflare | 20 دقيقة |
| 7 | تحديث كل bio بالرابط | 15 دقيقة |
| 8 | أول بوست يعلن الإطلاق | فوري |

**المجموع: يوم واحد من العمل الحقيقي.**

---

الانتشار في محركات البحث والذكاء الاصطناعي لا يأتي من سر.
يأتي من موقع موجود + محتوى منتشر + إشارات متكررة على الويب.
كل خطوة فوق = إشارة.
كل إشارة = ظهور إضافي.
ابدأ من الخطوة 1.
