# محدودیت options در TFSA

**با کارگزار، CRA، و مشاور مالیاتی چک کنید.** این صفحه نقشهٔ احتیاط از مستندات کارگزار است — نه مجوز معامله داخل TFSA.

!!! danger "توصیه مالی نیست"
    قوانین حساب registered از شرکتی به شرکت دیگر فرق می‌کند و عوض هم می‌شود.

## خلاصه

TFSA را پروفایل options **تنگ‌تر** از حساب margin به سبک آمریکا ببینید. برای مسیر کاری **PCS/CCS** در Spruce، تا وقتی کارگزار هر استراتژی را برای TFSA مکتوب تأیید نکرده، حساب **non-registered / margin** را جلو بگذارید.

چرا: در کارگزارهای بزرگ کانادایی، spreads چندپا معمولاً سطح options بالاتری می‌خواهند که به margin بند است؛ حساب registered پایین‌تر سقف می‌خورد.

## آنچه Interactive Brokers Canada نوشته

از [مجوزهای معاملهٔ TFSA در IBC](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php) (`[verified]` روی همان صفحه):

- داخل TFSA **margin نیست**؛ خرید باید کامل پرداخت شود؛ بدهی حساب مجاز نیست.  
- Options فهرست‌شده شامل equity call و put از نوع **long**، **covered calls**، و **protective puts** است.  
- **فرض نکنید** credit spreads در TFSA مربوط به IBC، بدون تأیید حساب خودتان، در دسترس‌اند.

## آنچه Questrade نوشته (یک نمونه)

از [سطوح options در Questrade](https://www.questrade.com/learning/using-questrade/options-levels) (`[verified]` روی همان صفحه):

- حساب‌های registered (TFSA / RRSP / FHSA) حداکثر **Level 2** می‌شوند.  
- **Spreads در Level 3**اند و حساب **margin** می‌خواهند.  
- Level 2 چیزهایی مثل covered call و cash-secured put را پوشش می‌دهد (با یادداشت) — نه مسیر CCS/PCS این playbookها.

کارگزارهای دیگر ممکن است فرق کنند. همیشه ماتریس *خودتان* را ببینید.

## معمولاً در TFSA محدود یا بسته

| Theme | چرا علامت می‌خورد |
|-------|--------------------|
| Short options از نوع naked / uncovered | ریسک شبیه margin؛ در کارگزارهای بررسی‌شدهٔ این‌جا در TFSA بسته است |
| Spreads چندپای short-premium | اغلب Level 3+ / فقط margin |
| قرض / اهرم داخل TFSA | مجاز نیست (IBC: داخل TFSA margin نیست) |
| معاملهٔ سفته‌بازانهٔ خیلی پرتکرار | CRA ممکن است بپرسد آیا کار شبیه کسب‌وکار است — از مشاور مالیاتی بپرسید |

## گاهی ممکن است (باز هم بسته به کارگزار)

| Theme | نکته |
|-------|--------|
| سهام / ETF از نوع long | واجد شرایط بودن محصول را چک کنید |
| Long calls / long puts | در فهرست TFSA مربوط به IBC؛ مسیر درآمد اصلی Spruce نیست |
| Covered call وقتی سهام دارید | در فهرست IBC؛ برای حساب خودتان تأیید بگیرید |
| Cash-secured puts | بسته به کارگزار؛ از بلاگ یک شرکت، قانون IBKR را نتیجه نگیرید |

## قبل از این‌که استراتژی را در TFSA تأمین مالی کنید

| Step | هدف |
|------|---------|
| هر استراتژی که ممکن است به‌کار ببرید را بنویسید (PCS، CCS، CSP، covered call، …) | چیزی را که نام نبرده‌اید نمی‌توانید تأیید کنید |
| از کارگزار بپرسید کدام‌ها در TFSA مجازند و کدام‌ها در margin | مکتوب یا screenshot از Client Portal بگیرید |
| جواب را خصوصی پیش خودتان نگه دارید | سایت عمومی جای جزئیات حساب نیست |
| [منابع](../00-meta/sources.md) را ورق بزنید | ببینید این خلاصه از کدام صفحات عمومی آمده |

## ادامه

- [کارگزارهای کانادایی](canadian-brokers.md)  
- [Cash یا margin](cash-vs-margin.md)  

## منابع

- [Interactive Brokers Canada — RRSP/TFSA information](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php)  
- [Questrade — Options levels](https://www.questrade.com/learning/using-questrade/options-levels)  
- [Wealthsimple — Options](https://www.wealthsimple.com/en-ca/trade/options)  
- [IBKR Campus — Options as part of an RRSP/TFSA strategy](https://www.interactivebrokers.com/campus/traders-insight/securities/options/options-as-part-of-an-rrsp-tfsa-strategy/)  

---

*توصیه مالی نیست. با کارگزار و CRA چک کنید.*
