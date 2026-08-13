# Playbook مربوط به put credit spread

این را بعد از [راه‌های مدیریت ریسک](../04-portfolio-and-risk/risk-management-categories.md) و [مثال مقایسه](../04-portfolio-and-risk/comparing-strategies-example.md) بخوانید. Put credit spread یک راه defined-risk برای گرفتن premium است، وقتی انتظار دارید سهام بالای short put بماند.

!!! danger "توصیه مالی نیست"
    فقط پیش‌نویس آموزشی است — توصیهٔ معاملهٔ هیچ نماد یا اندازه‌ای نیست.

## انتظار از ریسک و پاداش

Max loss برابر \(W - C\) اغلب از max profit برابر \(C\) **بزرگ‌تر** است. شکل معمول credit spread همین است: پاداش محدود، زیان defined بزرگ‌تر. اگر شکل برعکس می‌خواهید، در صفحهٔ مقایسه دوباره debit spreads را ببینید.

## کی این معامله با حرف شما جور است

Credit می‌گیرید وقتی thesis این است: *سهام باید بالای short put من بماند.* اگر اشتباه کنید، با تعریف max loss راحتید.

اگر آن جمله با نگاه شما نمی‌خواند، PCS را زور نکنید — [CCS](call-credit-spread-playbook.md) را ببینید یا کنار بایستید.

## ساختار (مرور سریع)

- Put در \(K_s\) بفروشید  
- Put در strike پایین‌تر \(K_l\) بخرید  
- Max profit \(\approx C\) (همان credit)  
- Max loss \(\approx W - C\) جایی که \(W = K_s - K_l\)  

نمودار کامل و مثال عددی: [Payoff مربوط به credit spread](../01-foundations/payoff-diagrams-credit-spreads.md).

## از ایده تا سفارش — هفت قدم

### ۱. Thesis

در یک یا دو جمله: چرا قیمت از short put پایین‌تر نمی‌رود؟ حمایت، کیفیت، valuation — هر چه فرآیندتان است — در journal جا دارد.

### ۲. Liquidity

نام‌ها و خطوط option با volume و open interest معقول را ترجیح دهید تا گیر bid/ask خیلی پهن نیفتید. کف عددی دقیق `[operator preference]` است.

### ۳. Expiration

با سوگیری monthly شروع کنید، مگر دلیلی برای weekly و اندازهٔ کوچک‌تر داشته باشید. ببینید [Weekly یا monthly](../01-foundations/expirations-weekly-monthly.md).

### ۴. Strikeها

منابع آموزشی رایج short premium را حوالی delta مطلق **0.15–0.30** بحث می‌کنند. `[verified]` به‌عنوان بازهٔ رایج. باند *خودتان* را روی کاغذ قفل کنید. Long put عرض را می‌گذارد و در نتیجه max loss را.

### ۵. Size

قرارداد را از **max loss** بشمارید، نه از قیمت سهم. خیلی از راهنماهای خرده‌فروشی نزدیک **۱–۲٪ از equity** در هر معامله را به‌عنوان باند آموزشی می‌گذارند. `[verified]` به‌عنوان راهنمایی رایج — سقف سخت شما شخصی است. بعد از fill هم **heat** را ببینید ([سیاست ریسک](../04-portfolio-and-risk/risk-policy.md)).

### ۶. رویدادها

اگر earnings (یا رویداد دوگانهٔ دیگر) داخل پنجرهٔ blackout شماست، رد کنید یا صبر کنید. Gap می‌تواند delta با دقت انتخاب‌شده را ندیده بگیرد.

### ۷. Journal

Thesis، strikeها، credit، max loss، و برچسب‌ها را بنویسید. خودِ چند ماه بعد بیشتر از یک یادداشت شلوغ روی نمودار به این‌ها نیاز دارد.

## اگر معامله بد پیش رفت

جعبهٔ جادویی برای تعمیر نیست. انتخاب‌های معمول:

- بستن با زیان defined  
- Roll (عوض کردن expiry یا strike) با چشم باز روی ریسک تازه  
- نگه داشتن تا نزدیک expiration، اگر همان سیاست مکتوب شماست  

*پیش‌فرض* را در روز آرام بنویسید، نه وقتی سهام دارد آبشاری پایین می‌آید.

## کارهایی که نکنید

- اندازه گرفتن چون «credit بزرگ به نظر می‌رسد»  
- روی‌هم چیدن PCS زیاد روی یک sector تا یک تم همه را با هم ببرد  
- «defined risk» را «ریسک کوچک» خواندن  
- long put را «فقط همین یک‌بار» حذف کردن

## بعد چه بخوانید

[Playbook مربوط به call credit spread](call-credit-spread-playbook.md) · [سیاست ریسک](../04-portfolio-and-risk/risk-policy.md)

## منابع

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان چک کنید.*
