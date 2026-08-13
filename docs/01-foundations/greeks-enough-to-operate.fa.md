# Greeks به‌اندازهٔ کار عملی

Greeks توصیف می‌کنند قیمت یک option معمولاً چگونه حرکت می‌کند. برای تصمیم‌های روزمره فقط چند تا لازم دارید.

!!! danger "توصیه مالی نیست"
    Greeks برآورد مبتنی بر مدل هستند — راهنما، نه تضمین.

## Delta

**Delta** تخمین می‌زند اگر سهام \$1 حرکت کند قیمت option چقدر جابه‌جا می‌شود، و اغلب به‌عنوان heuristic تقریبی «شانس تمام‌شدن in the money» به‌کار می‌رود. `[verified]` به‌عنوان تقریب گسترده‌آموزش‌داده‌شده.

- Long callها delta مثبت دارند؛ long putها delta منفی.  
- Short options علامت exposure شما را برعکس می‌کنند.  
- معامله‌گران اغلب strikeها را «20-delta» یا «30-delta» توصیف می‌کنند. بسیاری از منابع آموزشی short-premium strikeها را تقریباً در باند مطلق **0.15–0.30** بحث می‌کنند. `[verified]` به‌عنوان بازهٔ heuristic رایج — باند دقیق شما `[operator preference]` است.

Delta به **انتخاب strike** کمک می‌کند. جایگزین دستهٔ ریسک (sizing، spreads، coverage) نیست.

## Theta

**Theta** همان time decay است. Long options معمولاً برای زمان پول می‌دهند؛ short options اگر سهام همکاری کند ممکن است از زمان سود ببرند. نزدیک expiration، قیمت‌های نزدیک پول می‌توانند تند حرکت کنند — یکی از دلایل تطبیق expiration با تعداد دفعاتی که می‌توانید مرور کنید ([weekly در برابر monthly](expirations-weekly-monthly.md)).

## Implied volatility

**IV** حرکتی است که بازار قیمت‌گذاری کرده. IV بالاتر اغلب یعنی premium غنی‌تر و نوسان موردانتظار بزرگ‌تر. نزدیک **earnings**، IV اغلب بالا می‌رود و بعد از اعلام می‌تواند پایین بیاید — در حالی که سهام هنوز می‌تواند از strikeهای شما **gap** کند. `[verified]` به‌عنوان رفتار رایج رویداد.

## فعلاً چه را رد کنید

Gamma scalping عمیق، مدل‌سازی vol-surface، و rho.

## عادت

قبل از هر معامله — long، short، یا چندپا — بتوانید بگویید:

1. Delta / exposure جهتی من به زبان ساده چیست؟  
2. Max loss من به دلار چقدر است؟  
3. آیا رویدادی (earnings) داخل پنجره‌ام نشسته؟

## گام بعدی

[Weekly در برابر monthly](expirations-weekly-monthly.md) → [روش‌های مدیریت ریسک](../04-portfolio-and-risk/risk-management-categories.md).

## منابع

- [tastylive — Delta as a probability gauge](https://www.tastylive.com/news-insights/options-delta-predictive-probability-gauge-directional-measure)  
- [tastylive — IV crush](https://www.tastylive.com/concepts-strategies/iv-crush)  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان راستی‌آزمایی کنید.*
