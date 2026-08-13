# Greeks لازم برای کار

Greeks می‌گویند قیمت option معمولاً چطور حرکت می‌کند. برای کار روزمره چند تا کافی است.

!!! danger "توصیه مالی نیست"
    Greeks برآورد مدل‌اند — راهنما، نه تضمین.

## Delta

**Delta** تخمین می‌زند اگر سهام \$1 حرکت کند، قیمت option چقدر جابه‌جا می‌شود. خیلی‌ها از آن به‌عنوان تقریب «شانس تمام شدن in the money» هم استفاده می‌کنند. `[verified]` این تقریب در آموزش‌ها رایج است.

- Long call دلتای مثبت دارد؛ long put دلتای منفی.  
- Short option علامت exposure را برعکس می‌کند.  
- معامله‌گرها اغلب strike را «20-delta» یا «30-delta» صدا می‌کنند. در منابع آموزشی، short-premium معمولاً حوالی باند مطلق **0.15–0.30** بحث می‌شود. `[verified]` به‌عنوان بازهٔ رایج — باند دقیق شما `[operator preference]` است.

Delta برای **انتخاب strike** کمک می‌کند. جای sizing، spreads یا coverage را نمی‌گیرد.

## Theta

**Theta** همان time decay است. Long option معمولاً بابت زمان پول می‌دهد؛ short option اگر سهام همراهی کند ممکن است از زمان سود ببرد. نزدیک expiration، قیمت نزدیک پول می‌تواند تند حرکت کند — یکی از دلایل این‌که expiration را با تعداد دفعاتی که می‌توانید مرور کنید جور کنید ([weekly یا monthly](expirations-weekly-monthly.md)).

## Implied volatility

**IV** همان حرکتی است که بازار در قیمت گذاشته. IV بالاتر معمولاً یعنی premium گران‌تر و نوسان مورد انتظار بزرگ‌تر. نزدیک **earnings**، IV اغلب بالا می‌رود و بعد از اعلام ممکن است پایین بیاید — در حالی که سهام هنوز می‌تواند از strikeهای شما **gap** کند. `[verified]` این رفتار اطراف رویداد رایج است.

## فعلاً لازم نیست

Gamma scalping عمیق، مدل vol-surface، و rho.

## یک عادت ساده

قبل از هر معامله — long، short، یا چندپا — بتوانید بگویید:

1. Delta و جهت exposure من، به زبان ساده چیست؟  
2. Max loss من به دلار چقدر است؟  
3. آیا رویدادی مثل earnings داخل این پنجره هست؟

## بعد چه بخوانید

[Weekly یا monthly](expirations-weekly-monthly.md) → [راه‌های مدیریت ریسک](../04-portfolio-and-risk/risk-management-categories.md).

## منابع

- [tastylive — Delta as a probability gauge](https://www.tastylive.com/news-insights/options-delta-predictive-probability-gauge-directional-measure)  
- [tastylive — IV crush](https://www.tastylive.com/concepts-strategies/iv-crush)  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان چک کنید.*
