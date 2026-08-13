# Cash یا margin

Collateral و buying power را راحت می‌شود با «max loss» یکی گرفت. به هم مربوط‌اند، ولی یک عدد نیستند.

!!! danger "توصیه مالی نیست"
    Margin می‌تواند زیان را بزرگ کند و نقد اجباری راه بیندازد. شرایط را با کارگزارتان چک کنید.

## حساب cash، ساده

معمولاً موقعیت را با نقد تسویه‌شده می‌پردازید. Cash-secured put، جایی که مجاز باشد، یعنی نقد را برای assignment کنار می‌گذارید. این‌که spreads اصلاً مجاز باشند، باز هم به ماتریس تأیید کارگزار بستگی دارد.

## حساب margin، ساده

کارگزار زیر قوانین margin به شما buying power می‌دهد. Spreads از نوع defined-risk اغلب buying power کمتری از naked short می‌گیرند — این **یعنی معامله رایگان یا کوچک نیست**. **Max loss** ساختار و **margin requirement** کارگزار می‌توانند دو عدد مختلف باشند.

## صفحات کارگزار کانادایی برای Spruce چه می‌گویند

| مشاهده | معنی عملی | Tag |
|-------------|----------------------|-----|
| IBC: داخل TFSA **margin نیست** | معاملات چندپای شبیه margin را پیش‌فرض در TFSA نچینید | `[verified]` (صفحهٔ IBC) |
| Questrade: spreads **Level 3**اند و margin می‌خواهند؛ حساب registered تا Level 2 می‌ایستد | کار زندهٔ CCS/PCS معمولاً یعنی اول **margin / non-registered** | `[verified]` (صفحهٔ Questrade) |
| Naked short تأیید بالاتری می‌خواهد | با ممنوعیت این دوره روی ریسک naked برای معاملهٔ زنده جور است | الگوی رایج صنعت |

## ترجیح این دوره (پیش‌نویس)

| Preference | چرا |
|------------|-----|
| CCS/PCS را اول روی **non-registered margin** کار کنید | کارگزارهای کانادایی معمولاً spreads چندپا را همین‌طور محدود می‌کنند |
| TFSA را روی فهرست مجاز تنگ نگه دارید | با فهرست‌های option منتشرشدهٔ TFSA جور است |
| کنترل ریسک کارگزار را با API دور نزنید | شک دارید، معامله نکنید |

## Heat یا buying power

[Heat پرتفوی](../04-portfolio-and-risk/risk-policy.md) سقف خودتان نسبت به equity است. Buying power کارگزار سقف دوم است. هر دو باید جور باشند.

## ادامه

- [سیاست ریسک](../04-portfolio-and-risk/risk-policy.md)  
- [کارگزارهای کانادایی](canadian-brokers.md)  
- [محدودیت options در TFSA](tfsa-options-constraints.md)  
- [منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان چک کنید.*
