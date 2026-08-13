# Defined-risk credit spreads

تا این‌جا مکانیک options، دسته‌های ریسک، و مقایسهٔ دلاری را دیده‌اید. این صفحه می‌گوید **چرا مسیر کار Spruce credit spreads را جلو می‌گذارد** — نه این‌که تنها استراتژی دنیا باشند.

!!! danger "توصیه مالی نیست"
    اولویت یک سیستم شخصی، توصیه نیست که همه premium بفروشند.

## Credit spread کجای نقشه است

از [راه‌های مدیریت ریسک](../04-portfolio-and-risk/risk-management-categories.md):

- یک **spread** است (یک option، دیگری را hedge می‌کند).  
- ریسک **defined** است (max loss ≈ width − credit).  
- معمولاً **پاداش محدود** می‌دهد و اغلب **max loss &gt; max profit** — شکلی احتمال‌محور، نه بلیت بخت‌آزمایی.

ابزارهای درست دیگر روی همان نقشه: فقط sizing، covered call، cash-secured put، debit spread، protective put، سقف heat پرتفوی.

## چرا سیستم عملیاتی این‌ها را دوست دارد

برای مرور دسته‌ای و بعداً اتوماسیون، ساختار وقتی کمک می‌کند که:

1. Max loss همان موقع ورود مشخص باشد.  
2. ریسک صعود نامحدود naked در کار نباشد.  
3. Heat روی کل دفتر قابل جمع باشد.

Put credit spread (PCS) و call credit spread (CCS) همین قیدها را برآورده می‌کنند. این **ترجیح مهندسی** برای ops مربوط به Spruce است — بعد از آموزش، نه به‌جای آموزش.

## دو ساختار کاری

| View | Structure | داستان |
|------|-----------|-------|
| سهام باید بالای short put بماند | PCS / bull put | Credit می‌گیرید؛ ریسک سقوط با long put سقف دارد |
| سهام باید زیر short call بماند | CCS / bear call | Credit می‌گیرید؛ ریسک melt-up با long call سقف دارد |

ریاضی payoff: [Payoff مربوط به credit spread](../01-foundations/payoff-diagrams-credit-spreads.md).  
مقایسه با راه‌های دیگر: [مقایسهٔ استراتژی‌ها](../04-portfolio-and-risk/comparing-strategies-example.md).

## طرح کار

1. Thesis  
2. Expiration  
3. Strikeها → max loss → سیاست ریسک  
4. ورود یا رد  
5. Journal  
6. مدیریت با قوانینی که سر فرصت نوشته‌اید  

## یادداشت کانادایی

Spreads چندپا اغلب تأیید options بالاتر و حساب margin می‌خواهند. ببینید [محدودیت options در TFSA](../05-canadian-accounts/tfsa-options-constraints.md).

## Playbookها

- [Playbook مربوط به put credit spread](put-credit-spread-playbook.md)  
- [Playbook مربوط به call credit spread](call-credit-spread-playbook.md)  
- [پیش‌نویس سیاست ریسک](../04-portfolio-and-risk/risk-policy.md)  

## منابع

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان چک کنید.*
