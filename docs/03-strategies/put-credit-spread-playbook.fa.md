# Playbook مربوط به put credit spread

این را بعد از [روش‌های مدیریت ریسک](../04-portfolio-and-risk/risk-management-categories.md) و [مثال مقایسه](../04-portfolio-and-risk/comparing-strategies-example.md) به‌کار ببرید. یک put credit spread یک راه defined-risk برای جمع premium است وقتی انتظار دارید سهام بالای short put شما بماند.

!!! danger "توصیه مالی نیست"
    فقط پیش‌نویس آموزشی — توصیهٔ معاملهٔ هیچ نماد یا اندازه‌ای نیست.

## انتظار دربارهٔ ریسک در برابر پاداش

Max loss برابر \(W - C\) اغلب از max profit برابر \(C\) **بزرگ‌تر** است. این شکل معمول credit spread است (پاداش محدود، زیان defined بزرگ‌تر). اگر شکل برعکس می‌خواهید، debit spreads را در صفحهٔ مقایسه دوباره ببینید.

## وقتی این معامله با داستان شما جور است

وقتی thesis شما این است credit جمع می‌کنید: *سهام باید بالای short put من بماند.* اگر اشتباه کنید با تعریف max loss راحتید.

اگر آن جمله با نگاه شما جور نیست، PCS را زور نکنید — [CCS](call-credit-spread-playbook.md) را ببینید یا کنار بایستید.

## ساختار (مرور سریع)

- Put در \(K_s\) بفروشید  
- Put در strike پایین‌تر \(K_l\) بخرید  
- Max profit \(\approx C\) (همان credit)  
- Max loss \(\approx W - C\) جایی که \(W = K_s - K_l\)  

نمودار کامل و مثال عددی: [Payoffهای credit spread](../01-foundations/payoff-diagrams-credit-spreads.md).

## از ایده تا سفارش — هفت گام

### ۱. Thesis

در یک یا دو جمله: چرا قیمت از short put سقوط نمی‌کند؟ حمایت، کیفیت، valuation — هر چه فرآیندتان به‌کار می‌برد — در journal جا دارد.

### ۲. Liquidity

نام‌ها و خطوط option با volume و open interest معقول را ترجیح دهید تا با bid/askهای خیلی پهن نجنگید. کف‌های عددی دقیق `[operator preference]` هستند.

### ۳. Expiration

با سوگیری monthly شروع کنید مگر دلیلی برای weekly و اندازهٔ کوچک‌تر داشته باشید. ببینید [Weekly در برابر monthly](../01-foundations/expirations-weekly-monthly.md).

### ۴. Strikeها

مطالب آموزشی رایج short premium را حول delta مطلق **0.15–0.30** بحث می‌کنند. `[verified]` به‌عنوان بازهٔ heuristic رایج. باند *خودتان* را مکتوب قفل کنید. Long put عرض و بنابراین max loss را می‌گذارد.

### ۵. Size

قراردادها را از **max loss** بشمارید، نه از قیمت سهم. بسیاری از راهنماهای خرده‌فروشی نزدیک **۱–۲٪ از equity** به‌ازای معامله را به‌عنوان باند آموزشی شروع می‌کنند. `[verified]` به‌عنوان راهنمایی رایج — سقف سخت شما شخصی است. بعد از fill هم **heat** را چک کنید (ببینید [سیاست ریسک](../04-portfolio-and-risk/risk-policy.md)).

### ۶. رویدادها

اگر earnings (یا رویداد باینری دیگر) داخل پنجرهٔ blackout شماست، رد کنید یا صبر کنید. Gap می‌تواند delta با دقت انتخاب‌شده را نادیده بگیرد.

### ۷. Journal

Thesis، strikeها، credit، max loss، و برچسب‌ها را ثبت کنید. خودِ آینده بیشتر از یک annotation کامل نمودار به آن نیاز دارد.

## اگر معامله غلط برود

کیت تعمیر جادویی نیست. انتخاب‌های معمول:

- بستن با زیان defined  
- Roll (عوض کردن expiry/strike) با چشم باز روی ریسک جدید  
- نگه داشتن به‌سوی expiration اگر آن سیاست مکتوب شماست  

*پیش‌فرض* را در روز آرام تصمیم بگیرید، نه وقتی سهام در حال ریزش آبشاری است.

## ضدالگوها

- اندازه‌گذاری چون «credit بزرگ به نظر می‌رسد»  
- روی‌هم‌چیدن PCSهای زیاد روی همان sector تا یک تم همه را غرق کند  
- رفتار با «defined risk» به‌عنوان «ریسک کوچک»  
- رد کردن long put «فقط همین یک‌بار»

## گام بعدی

[Playbook مربوط به call credit spread](call-credit-spread-playbook.md) · [سیاست ریسک](../04-portfolio-and-risk/risk-policy.md)

## منابع

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان راستی‌آزمایی کنید.*
