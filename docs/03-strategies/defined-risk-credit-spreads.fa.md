# Defined-risk credit spreads

تا اینجا مکانیک options، دسته‌های ریسک، و مقایسهٔ دلاری کنارهم را دیده‌اید. این صفحه توضیح می‌دهد **چرا مسیر عملیاتی Spruce credit spreads را اولویت می‌دهد** — نه این‌که تنها استراتژی موجود باشند.

!!! danger "توصیه مالی نیست"
    اولویت برای یک سیستم عملیاتی شخصی توصیه نیست که همه باید premium بفروشند.

## Credit spreads کجای نقشه می‌نشینند

از [روش‌های مدیریت ریسک](../04-portfolio-and-risk/risk-management-categories.md):

- یک **spread** هستند (یک option دیگری را hedge می‌کند).  
- ریسک **defined** است (max loss ≈ width − credit).  
- معمولاً **پاداش محدود** می‌دهند و اغلب **max loss &gt; max profit** — شکلی احتمال‌محور، نه بلیت بخت‌آزمایی.

ابزارهای معتبر دیگر روی همان نقشه: فقط sizing، covered calls، cash-secured puts، debit spreads، protective puts، سقف‌های heat پرتفوی.

## چرا یک سیستم عملیاتی آن‌ها را دوست دارد

برای مرور دسته‌ای و اتوماسیون بعدی، ساختار وقتی کمک می‌کند که:

1. Max loss در ورود مشخص باشد.  
2. ریسک صعود نامحدود naked اجتناب شود.  
3. Heat روی دفتر قابل جمع باشد.

Put credit spreads (PCS) و call credit spreads (CCS) این قیدها را برآورده می‌کنند. این یک **ترجیح مهندسی** برای ops مربوط به Spruce است — بعد از آموزش، نه به‌جای آموزش.

## دو ساختار کاری

| View | Structure | داستان |
|------|-----------|-------|
| سهام باید بالای short put بماند | PCS / bull put | Credit جمع کنید؛ ریسک سقوط با long put سقف دارد |
| سهام باید زیر short call بماند | CCS / bear call | Credit جمع کنید؛ ریسک melt-up با long call سقف دارد |

ریاضی payoff: [Payoffهای credit spread](../01-foundations/payoff-diagrams-credit-spreads.md).  
مقایسهٔ منصفانه با رویکردهای دیگر: [مقایسهٔ استراتژی‌ها](../04-portfolio-and-risk/comparing-strategies-example.md).

## طرح فرآیند

1. Thesis  
2. Expiration  
3. Strikeها → max loss → سیاست ریسک  
4. ورود یا رد  
5. Journal  
6. مدیریت با قوانینی که آرام نوشته شده‌اند  

## یادداشت کانادایی

Spreads چندپا اغلب به تأیید options بالاتر و حساب margin نیاز دارند. ببینید [محدودیت‌های TFSA](../05-canadian-accounts/tfsa-options-constraints.md).

## Playbookها

- [Playbook مربوط به put credit spread](put-credit-spread-playbook.md)  
- [Playbook مربوط به call credit spread](call-credit-spread-playbook.md)  
- [پیشنهاد سیاست ریسک](../04-portfolio-and-risk/risk-policy.md)  

## منابع

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان راستی‌آزمایی کنید.*
