# 💻 SEO Code Snippets - أكواد جاهزة للاستخدام
## Copy-Paste Ready SEO Codes

---

## 📄 1. Meta Tags Template (عام)

استخدم هذا الـ Template لأي صفحة جديدة:

```html
<!-- ===== META BASICS ===== -->
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="language" content="ar">
 
<!-- ===== TITLE & DESCRIPTION ===== -->
<title>[PAGE_TITLE] | المحمدي - نقل عفش القصيم</title>
<meta name="description" content="[PAGE_DESCRIPTION] - شركة المحمدي المتخصصة في نقل العفش والأثاث بالقصيم">

<!-- ===== KEYWORDS ===== -->
<meta name="keywords" content="[PRIMARY_KEYWORD], [SECONDARY_KEYWORD], المحمدي, نقل عفش, القصيم">

<!-- ===== CANONICAL URL ===== -->
<link rel="canonical" href="https://almohannadi-movers.sa/[page-slug]">

<!-- ===== OPEN GRAPH TAGS ===== -->
<meta property="og:type" content="website">
<meta property="og:title" content="[PAGE_TITLE]">
<meta property="og:description" content="[PAGE_DESCRIPTION]">
<meta property="og:url" content="https://almohannadi-movers.sa/[page-slug]">
<meta property="og:image" content="https://almohannadi-movers.sa/images/og-image.jpg">
<meta property="og:locale" content="ar_SA">

<!-- ===== TWITTER CARDS ===== -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="[PAGE_TITLE]">
<meta name="twitter:description" content="[PAGE_DESCRIPTION]">
<meta name="twitter:image" content="https://almohannadi-movers.sa/images/og-image.jpg">

<!-- ===== ADDITIONAL META ===== -->
<meta name="robots" content="index, follow">
<meta name="author" content="شركة المحمدي">
```

---

## 🏢 2. LocalBusiness Schema (للصفحات المحلية)

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "شركة المحمدي لنقل العفش والأثاث",
  "image": "https://almohannadi-movers.sa/logo.png",
  "description": "[CITY_NAME] - نقل عفش احترافي وآمن",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "[STREET_ADDRESS]",
    "addressLocality": "[CITY_NAME]",
    "addressRegion": "القصيم",
    "postalCode": "[POSTAL_CODE]",
    "addressCountry": "SA"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": "[LATITUDE]",
    "longitude": "[LONGITUDE]"
  },
  "telephone": "0582717472",
  "url": "https://almohannadi-movers.sa/[page-slug]",
  "openingHoursSpecification": {
    "@type": "OpeningHoursSpecification",
    "dayOfWeek": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"],
    "opens": "07:00",
    "closes": "24:00"
  },
  "sameAs": [
    "https://www.facebook.com/almohannadi",
    "https://www.instagram.com/almohannadi",
    "https://www.tiktok.com/@almohannadi"
  ]
}
</script>
```

---

## 🏙️ 3. City Page Template (صفحة مدينة)

هذا template يمكن نسخه لكل مدينة (بريدة، عنيزة، الرس، إلخ):

```html
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<!-- استخدم Template من القسم 1 -->
<!-- غير:
  [PAGE_TITLE] = نقل عفش بـ [CITY_NAME] | المحمدي
  [PAGE_DESCRIPTION] = نقل عفش احترافي في [CITY_NAME]...
  [PRIMARY_KEYWORD] = نقل عفش بـ [CITY_NAME]
-->
</head>
<body>
  <main>
    <section class="hero">
      <h1>نقل العفش والأثاث ب[CITY_NAME] - شركة المحمدي</h1>
      <p>أكثر من 12 سنة خبرة في نقل العفش والأثاث في [CITY_NAME]</p>
    </section>
    
    <section class="services">
      <h2>خدماتنا في [CITY_NAME]</h2>
      <p>نوفر خدمات نقل عفش متكاملة...</p>
    </section>

    <section class="testimonials">
      <h2>تقييمات عملائنا من [CITY_NAME]</h2>
      <!-- أضف تقييمات حقيقية من السكان المحليين -->
    </section>

    <section class="faq">
      <h2>أسئلة شائعة عن نقل العفش في [CITY_NAME]</h2>
      <!-- استخدم FAQPage Schema من القسم 5 -->
    </section>
  </main>
</body>
</html>
```

---

## 🖼️ 4. Responsive Image Code

```html
<!-- استخدم هذا لكل صورة -->
<picture>
  <source media="(min-width: 1200px)" srcset="image-lg.webp" type="image/webp">
  <source media="(min-width: 768px)" srcset="image-md.webp" type="image/webp">
  <source media="(max-width: 767px)" srcset="image-sm.webp" type="image/webp">
  
  <!-- Fallback -->
  <source srcset="image.webp" type="image/webp">
  <img src="image.jpg" 
       alt="[DESCRIPTIVE_ALT_TEXT]" 
       loading="lazy"
       width="[WIDTH]"
       height="[HEIGHT]"
       decoding="async">
</picture>
```

---

## 📋 5. FAQPage Schema

استخدم هذا لإضافة الأسئلة الشائعة:

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "[QUESTION_1]",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[ANSWER_1]"
      }
    },
    {
      "@type": "Question",
      "name": "[QUESTION_2]",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[ANSWER_2]"
      }
    }
  ]
}
</script>
```

**مثال بيانات فعلية:**
```json
{
  "@type": "Question",
  "name": "كم تكلفة نقل العفش من بريدة إلى الرياض؟",
  "acceptedAnswer": {
    "@type": "Answer",
    "text": "السعر يتراوح بين 500 إلى 1500 ريال حسب حجم العفش. اتصل بنا على 0582717472 للحصول على عرض سعر مجاني."
  }
}
```

---

## ⭐ 6. Review Schema

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org/",
  "@type": "Review",
  "itemReviewed": {
    "@type": "LocalBusiness",
    "name": "شركة المحمدي لنقل العفش"
  },
  "reviewRating": {
    "@type": "Rating",
    "ratingValue": "[RATING: 1-5]",
    "bestRating": "5",
    "worstRating": "1"
  },
  "author": {
    "@type": "Person",
    "name": "[REVIEWER_NAME]"
  },
  "reviewBody": "[REVIEW_TEXT]",
  "datePublished": "[DATE_YYYY-MM-DD]"
}
</script>
```

**مثال:**
```json
{
  "reviewRating": {
    "ratingValue": "5"
  },
  "author": {
    "name": "محمد الشمري"
  },
  "reviewBody": "خدمة ممتازة جداً، فريق محترف والأسعار شفافة!",
  "datePublished": "2025-06-15"
}
```

---

## 🎯 7. Video Schema

إذا أضفت مقاطع فيديو:

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "VideoObject",
  "name": "[VIDEO_TITLE]",
  "description": "[VIDEO_DESCRIPTION]",
  "thumbnailUrl": "https://almohannadi-movers.sa/images/thumb.jpg",
  "uploadDate": "[DATE_YYYY-MM-DD]",
  "duration": "PT[MM]M[SS]S",
  "contentUrl": "https://almohannadi-movers.sa/videos/[video-name].mp4",
  "embedUrl": "https://almohannadi-movers.sa/videos/[video-name].html"
}
</script>
```

---

## 💬 8. Testimonial Section HTML

```html
<section class="testimonials">
  <h2>ماذا يقول عملاؤنا</h2>
  
  <div class="testimonial" itemscope itemtype="https://schema.org/Review">
    <div class="stars">★★★★★</div>
    <p itemprop="reviewBody">
      "فريق محترف جداً، التزموا بالموعد، وكل الأثاث وصل سليم!"
    </p>
    <p class="author" itemprop="author">
      - <strong>محمد الشمري</strong> من بريدة
    </p>
    <meta itemprop="ratingValue" content="5">
  </div>

  <div class="testimonial" itemscope itemtype="https://schema.org/Review">
    <div class="stars">★★★★★</div>
    <p itemprop="reviewBody">
      "أول مرة أستخدم خدمات نقل عفش، كانت تجربة رائعة جداً."
    </p>
    <p class="author" itemprop="author">
      - <strong>نورة العيسى</strong> من عنيزة
    </p>
    <meta itemprop="ratingValue" content="5">
  </div>
</section>
```

---

## 🔗 9. Internal Linking Best Practices

```html
<!-- ❌ تجنب: -->
<a href="#services">اضغط هنا</a>

<!-- ✅ استخدم: -->
<a href="#services">اكتشف خدمات نقل العفش المتخصصة</a>

<!-- في Hero: -->
<a href="#services">تعرف على خدماتنا المتميزة</a>

<!-- في About: -->
<a href="#gallery">شاهد أعمالنا الفعلية في الميدان</a>

<!-- في Footer: -->
<a href="#why">استكشف لماذا نختلف عن الآخرين</a>
```

---

## 📍 10. Breadcrumb Navigation HTML

```html
<nav aria-label="Breadcrumb">
  <ol itemscope itemtype="https://schema.org/BreadcrumbList">
    <li itemprop="itemListElement" itemscope itemtype="https://schema.org/ListItem">
      <a itemprop="item" href="https://almohannadi-movers.sa/">
        <span itemprop="name">الرئيسية</span>
      </a>
      <meta itemprop="position" content="1">
    </li>
    <li itemprop="itemListElement" itemscope itemtype="https://schema.org/ListItem">
      <a itemprop="item" href="https://almohannadi-movers.sa/#services">
        <span itemprop="name">الخدمات</span>
      </a>
      <meta itemprop="position" content="2">
    </li>
    <li itemprop="itemListElement" itemscope itemtype="https://schema.org/ListItem">
      <span itemprop="name">نقل العفش</span>
      <meta itemprop="position" content="3">
    </li>
  </ol>
</nav>
```

---

## 🤖 11. Robots.txt Entries

```robots.txt
# لمنع فهرسة صفحة معينة:
User-agent: *
Disallow: /private-page/

# للسماح بفهرسة ملف معين فقط:
User-agent: *
Allow: /important-page.html
Disallow: /

# لتعيين Crawl-delay:
User-agent: Googlebot
Crawl-delay: 1

# لمنع فهرسة صور معينة:
User-agent: *
Disallow: /images/private/
```

---

## 🗺️ 12. Sitemap.xml Entry Template

```xml
<url>
  <loc>https://almohannadi-movers.sa/[page-slug]</loc>
  <lastmod>2025-06-22T12:00:00Z</lastmod>
  <changefreq>weekly</changefreq>
  <priority>0.8</priority>
  <mobile:mobile/>
  
  <image:image>
    <image:loc>https://almohannadi-movers.sa/images/image.jpg</image:loc>
    <image:title>[IMAGE_TITLE]</image:title>
  </image:image>
</url>
```

---

## 🎨 13. CSS للـ SEO

```css
/* Hide text visually but keep it for screen readers */
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  border-width: 0;
}

/* Focus visible for keyboard navigation (SEO-friendly) */
a:focus-visible,
button:focus-visible {
  outline: 2px solid #e8590c;
  outline-offset: 2px;
}

/* Improve readability */
body {
  line-height: 1.6;
  font-size: 16px;
}

h1, h2, h3 {
  margin-top: 1em;
  margin-bottom: 0.5em;
}
```

---

## 📊 14. Google Analytics 4 Tracking Code

```html
<!-- أضف هذا قبل </head> -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXX');
  
  // Track phone clicks
  gtag('event', 'phone_click', {
    'phone_number': '0582717472'
  });
</script>
```

---

## 📞 15. Contact Schema

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "شركة المحمدي",
  "url": "https://almohannadi-movers.sa",
  "contactPoint": {
    "@type": "ContactPoint",
    "contactType": "Customer Service",
    "telephone": "0582717472",
    "email": "contact@almohannadi-movers.sa",
    "areaServed": "SA",
    "availableLanguage": ["ar", "en"]
  }
}
</script>
```

---

## ✅ Verification Checklist

استخدم هذه القائمة للتحقق من التحسينات:

```
□ Title Tag يحتوي على 50-60 حرف
□ Meta Description يحتوي على 150-160 حرف
□ H1 واحد فقط في الصفحة
□ Alt Text لجميع الصور
□ Internal Links لا أقل من 3 روابط
□ Mobile-responsive design
□ Page Speed > 90 (PageSpeed Insights)
□ HTTPS enabled
□ JSON-LD Structured Data موجود
□ Robots.txt و Sitemap.xml موجودة
□ Canonical URL موجود
□ No Broken Links
□ Google Business Profile محدّث
□ Google Search Console متصل
```

---

**ملاحظة**: استبدل `[PLACEHOLDER]` بالقيم الفعلية عند استخدام أي snippet.

آخر تحديث: 22 يونيو 2025
