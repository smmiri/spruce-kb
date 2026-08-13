# Playbook مربوط به call credit spread

این را بعد از صفحات مدیریت ریسک به‌کار ببرید. یک call credit spread وقتی premium جمع می‌کند که انتظار دارید سهام زیر short call شما بماند — با long call که ریسک melt-up را سقف می‌گذارد.

!!! danger "توصیه مالی نیست"
    فقط پیش‌نویس آموزشی — توصیهٔ معاملهٔ هیچ نماد یا اندازه‌ای نیست.

## انتظار دربارهٔ ریسک در برابر پاداش

مثل دیگر credit spreads، max loss اغلب از max profit بیشتر است. این طراحی عمدی پاداش محدود است، نه مثال خراب. Naked short callها سقف را کاملاً برمی‌دارند و می‌توانند بدون حد زیان بدهند. `[verified]`

## وقتی این معامله با داستان شما جور است

وقتی thesis شما این است credit جمع می‌کنید: *سهام باید زیر short call من بماند.* اغلب نامی است که از قبل کشیده، گران، یا بعید به نظر می‌رسد در کوتاه‌مدت به بالا رفتن ادامه دهد — هنوز thesisای که باید بنویسید، نه حس.

اگر نیاز دارید سهام بالا برود، این ابزار غلط است. [PCS](put-credit-spread-playbook.md) را در نظر بگیرید یا معامله نکنید.

!!! tip "چرا spread به‌جای naked short call؟"
    یک naked short call اگر سهام به بالا رفتن ادامه دهد می‌تواند از نظر نظری مبلغ نامحدود زیان بدهد. `[verified]` Long call در CCS همان سقف است.

## ساختار (مرور سریع)

- Call در \(K_s\) بفروشید  
- Call در strike بالاتر \(K_h\) بخرید  
- Max profit \(\approx C\)  
- Max loss \(\approx W - C\) جایی که \(W = K_h - K_s\)  

نمودارها: [Payoffهای credit spread](../01-foundations/payoff-diagrams-credit-spreads.md).

## از ایده تا سفارش — هفت گام

### ۱. Thesis

چرا قیمت از short call melt-up نمی‌کند؟ در journal بنویسید.

### ۲. Liquidity

همان معیار PCS — زنجیره‌های option را که نمی‌توانید تمیز خارج شوید رد کنید.

### ۳. Expiration

سوگیری monthly؛ weeklies فقط با اندازهٔ تنگ‌تر.

### ۴. Strikeها

Short call در باند delta که از قبل انتخاب کرده‌اید (بازهٔ آموزشی رایج حدود 0.15–0.30 delta مطلق). `[verified]` به‌عنوان heuristic. Long call عرض و max loss را می‌گذارد.

### ۵. Size

از max loss و heat پرتفوی استفاده کنید — نه «درصد حسابی که در premium نشسته.» اعداد سیاست در [صفحهٔ ریسک](../04-portfolio-and-risk/risk-policy.md) هستند.

### ۶. رویدادها

Blackout مربوط به earnings / رویداد را در سیاست‌تان رعایت کنید.

### ۷. Journal

شامل این باشد که چرا CCS را به‌جای PCS انتخاب کردید (یا چرا هر دو روی نام‌های مختلف ظاهر می‌شوند).

## اگر معامله غلط برود

همان منوی صادقانهٔ PCS: بستن، roll، یا نگه داشتن زیر قوانینی که وقتی آرام بودید نوشتید. روندهای قوی می‌توانند دورتر از آنچه یک credit کوچک «حس می‌کند» باید اجازه دهد بدوند.

## ضدالگوها

- Naked short call چون «تقریباً spread فروختم»  
- بسیاری از موقعیت‌های CCS همبسته که در واقع یک شرط بزرگ tech هستند  
- نادیده گرفتن این‌که squeeze می‌تواند سریع short strike شما را بزند

## گام بعدی

[پیشنهاد سیاست ریسک](../04-portfolio-and-risk/risk-policy.md) · [نمای کلی defined-risk](defined-risk-credit-spreads.md)

## منابع

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- افشاهای OCC / کارگزار دربارهٔ uncovered call writing  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان راستی‌آزمایی کنید.*
