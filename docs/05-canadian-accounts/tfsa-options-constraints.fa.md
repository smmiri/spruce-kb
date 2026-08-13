# محدودیت‌های TFSA برای options

**با کارگزار، CRA، و مشاور مالیاتی راستی‌آزمایی کنید.** این صفحه نقشهٔ احتیاط از مستندات کارگزار است — نه مجوز معاملهٔ یک استراتژی داخل TFSA.

!!! danger "توصیه مالی نیست"
    قوانین حساب registered بسته به شرکت فرق می‌کند و در زمان عوض می‌شود.

## نسخهٔ کوتاه

TFSA را پروفایل options **تنگ‌تر** از حساب margin به سبک آمریکا ببینید. برای فرآیند کاری **PCS/CCS** مربوط به Spruce، تا وقتی کارگزار هر استراتژی را برای TFSA مکتوب تأیید کند، حساب **non-registered / margin** را ترجیح دهید.

چرا: در کارگزارهای بزرگ کانادایی، spreads چندپا اغلب در سطح options بالاتری می‌نشینند که به margin نیاز دارد، در حالی که حساب‌های registered پایین‌تر سقف می‌خورند.

## آنچه Interactive Brokers Canada منتشر می‌کند

از [مجوزهای معاملهٔ TFSA مربوط به IBC](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php) (`[verified]` در برابر آن صفحه):

- **بدون margin** در TFSA؛ خریدها کامل پرداخت می‌شوند؛ بدهی حساب مجاز نیست.  
- Options فهرست‌شده شامل equity call و put از نوع **long**، **covered calls**، و **protective puts** هستند.  
- **فرض نکنید** credit spreads در TFSA مربوط به IBC بدون تأیید برای حساب شما در دسترس‌اند.

## آنچه Questrade منتشر می‌کند (مثال صنعت)

از [سطوح options مربوط به Questrade](https://www.questrade.com/learning/using-questrade/options-levels) (`[verified]` در برابر آن صفحه):

- حساب‌های registered (TFSA / RRSP / FHSA) حداکثر در **Level 2** تمام می‌شوند.  
- **Spreads در Level 3** هستند و به حساب **margin** نیاز دارند.  
- Level 2 ایده‌هایی مثل covered calls و cash-secured puts را پوشش می‌دهد (با یادداشت) — نه مسیر CCS/PCS که این playbookها توصیف می‌کنند.

کارگزارهای دیگر ممکن است فرق کنند. همیشه ماتریس *خودتان* را چک کنید.

## معمولاً در TFSA محدود یا مسدود

| Theme | چرا افراد علامت می‌گذارند |
|-------|--------------------|
| Short options از نوع naked / uncovered | ریسک سبک margin؛ در TFSA در کارگزارهای بررسی‌شده اینجا مسدود است |
| Spreads چندپای short-premium | اغلب Level 3+ / فقط margin |
| قرض / اهرم داخل TFSA | مجاز نیست (IBC: بدون margin در TFSA) |
| معاملهٔ سفته‌بازانهٔ خیلی مکرر | CRA ممکن است بپرسد آیا فعالیت شبیه کسب‌وکار به نظر می‌رسد — از مشاور مالیاتی بپرسید |

## گاهی قابل کار (هنوز وابسته به کارگزار)

| Theme | Caveat |
|-------|--------|
| سهام / ETF از نوع long | واجد شرایط بودن محصول را تأیید کنید |
| Long calls / long puts | در فهرست TFSA مربوط به IBC؛ فرآیند درآمد اصلی Spruce نیست |
| Covered calls وقتی سهام دارید | در فهرست IBC؛ برای حساب خودتان تأیید کنید |
| Cash-secured puts | وابسته به کارگزار؛ IBKR را از بلاگ شرکت دیگر استنباط نکنید |

## قبل از تأمین مالی یک استراتژی در TFSA

| Step | هدف |
|------|---------|
| هر استراتژی که ممکن است به‌کار ببرید را فهرست کنید (PCS، CCS، CSP، covered call، …) | نمی‌توانید چیزی را تأیید کنید که نام نبرده‌اید |
| از کارگزار بپرسید کدام‌ها در TFSA در برابر margin مجازند | مکتوب یا screenshot از Client Portal بگیرید |
| آن جواب را خصوصی با سوابق خود نگه دارید | سایت‌های عمومی نباید جزئیات حساب شما را نگه دارند |
| [منابع](../00-meta/sources.md) را مرور کنید | بدانید کدام صفحات عمومی برای این خلاصه به‌کار رفته‌اند |

## مطالعهٔ مرتبط

- [کارگزارهای کانادایی](canadian-brokers.md)  
- [Cash در برابر margin](cash-vs-margin.md)  

## منابع

- [Interactive Brokers Canada — RRSP/TFSA information](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php)  
- [Questrade — Options levels](https://www.questrade.com/learning/using-questrade/options-levels)  
- [Wealthsimple — Options](https://www.wealthsimple.com/en-ca/trade/options)  
- [IBKR Campus — Options as part of an RRSP/TFSA strategy](https://www.interactivebrokers.com/campus/traders-insight/securities/options/options-as-part-of-an-rrsp-tfsa-strategy/)  

---

*توصیه مالی نیست. با کارگزار و CRA راستی‌آزمایی کنید.*
