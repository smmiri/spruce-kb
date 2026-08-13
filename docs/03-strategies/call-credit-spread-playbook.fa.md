# Playbook مربوط به call credit spread

این را بعد از صفحه‌های مدیریت ریسک بخوانید. Call credit spread وقتی premium می‌گیرد که انتظار دارید سهام زیر short call بماند — و long call ریسک melt-up را سقف می‌گذارد.

!!! danger "توصیه مالی نیست"
    فقط پیش‌نویس آموزشی است — توصیهٔ معاملهٔ هیچ نماد یا اندازه‌ای نیست.

## انتظار از ریسک و پاداش

مثل بقیهٔ credit spreads، max loss اغلب از max profit بیشتر است. این طراحی عمدی پاداش محدود است، نه مثال خراب. Naked short call سقف را برمی‌دارد و می‌تواند بی‌حد زیان بدهد. `[verified]`

## کی این معامله با حرف شما جور است

Credit می‌گیرید وقتی thesis این است: *سهام باید زیر short call من بماند.* اغلب نامی است که کش آمده، گران شده، یا بعید است در کوتاه‌مدت همین‌طور بالا برود — باز هم thesis است که باید بنویسید، نه حس.

اگر لازم دارید سهام بالا برود، این ابزار غلط است. [PCS](put-credit-spread-playbook.md) را ببینید یا معامله نکنید.

!!! tip "چرا spread، نه naked short call؟"
    Naked short call اگر سهام به بالا رفتن ادامه دهد، از نظر نظری می‌تواند بی‌حد زیان بدهد. `[verified]` Long call در CCS همان سقف است.

## ساختار (مرور سریع)

- Call در \(K_s\) بفروشید  
- Call در strike بالاتر \(K_h\) بخرید  
- Max profit \(\approx C\)  
- Max loss \(\approx W - C\) جایی که \(W = K_h - K_s\)  

نمودارها: [Payoff مربوط به credit spread](../01-foundations/payoff-diagrams-credit-spreads.md).

## از ایده تا سفارش — هفت قدم

### ۱. Thesis

چرا قیمت از short call بالا نمی‌زند؟ در journal بنویسید.

### ۲. Liquidity

همان معیار PCS — زنجیره‌ای که نمی‌توانید تمیز ازش بیرون بیایید را رد کنید.

### ۳. Expiration

سوگیری monthly؛ weeklies فقط با اندازهٔ تنگ‌تر.

### ۴. Strikeها

Short call در باند delta که از قبل انتخاب کرده‌اید (بازهٔ آموزشی رایج حدود 0.15–0.30 delta مطلق). `[verified]` به‌عنوان heuristic. Long call عرض و max loss را می‌گذارد.

### ۵. Size

از max loss و heat پرتفوی استفاده کنید — نه «چند درصد حساب در premium نشسته.» عددهای سیاست در [صفحهٔ ریسک](../04-portfolio-and-risk/risk-policy.md) است.

### ۶. رویدادها

Blackout مربوط به earnings و رویداد را در سیاست‌تان رعایت کنید.

### ۷. Journal

بنویسید چرا CCS را به‌جای PCS انتخاب کردید (یا چرا هر دو روی نام‌های مختلف نشسته‌اند).

## اگر معامله بد پیش رفت

همان منوی صادقانهٔ PCS: بستن، roll، یا نگه داشتن زیر قوانینی که وقتی آرام بودید نوشتید. روند قوی می‌تواند خیلی دورتر از آنچه یک credit کوچک «حس می‌کند» باید تحمل کند، بدود.

## کارهایی که نکنید

- Naked short call چون «تقریباً spread فروختم»  
- چند CCS همبسته که در واقع یک شرط بزرگ tech است  
- نادیده گرفتن این‌که squeeze می‌تواند سریع short strike را بزند

## بعد چه بخوانید

[پیش‌نویس سیاست ریسک](../04-portfolio-and-risk/risk-policy.md) · [نمای کلی defined-risk](defined-risk-credit-spreads.md)

## منابع

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- افشاهای OCC / کارگزار دربارهٔ uncovered call writing  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان چک کنید.*
