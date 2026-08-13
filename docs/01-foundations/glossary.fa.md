# Glossary

تعاریف به زبان ساده. یک‌بار مرور کنید، بعد هر وقت صفحه‌ای اصطلاحی به‌کار برد که یادتان نماند برگردید.

نام اصطلاح‌ها به English می‌مانند؛ توضیح‌ها به فارسی است.

!!! danger "توصیه مالی نیست"
    فقط تعاریف آموزشی.

## بلوک‌های سازنده

| Term | معنی ساده |
|------|----------------|
| **Call** | قراردادی با حق **خرید** سهام در strike. |
| **Put** | قراردادی با حق **فروش** سهام در strike. |
| **Premium** | قیمت option (یا net credit/debit یک معاملهٔ چندپا). |
| **Strike** | قیمتی که در قرارداد نام برده شده. |
| **Expiration** | زمانی که قرارداد تمام می‌شود. |
| **ITM** | In the money — برای call وقتی سهام بالای strike است؛ برای put وقتی سهام پایین strike است. |
| **OTM** | Out of the money — برعکس ITM. |
| **ATM** | At the money — سهام نزدیک strike. |

## Spreads و شکل ریسک

| Term | معنی ساده |
|------|----------------|
| **Credit spread** | یک معاملهٔ چندپای options باز می‌کنید و **net credit** می‌گیرید. معمولاً یک short option به‌علاوهٔ یک long option برای حفاظت. |
| **PCS / put credit spread** | یک put می‌فروشید، یک put پایین‌تر می‌خرید. به آن **bull put spread** هم می‌گویند. می‌خواهید سهام بالای short put بماند. |
| **CCS / call credit spread** | یک call می‌فروشید، یک call بالاتر می‌خرید. به آن **bear call spread** هم می‌گویند. می‌خواهید سهام زیر short call بماند. |
| **Defined risk** | بدترین زیان را از روی ساختار در ورود می‌دانید (قبل از کارمزد). |
| **Undefined risk** | زیان می‌تواند بدون سقف ساختاری تمیز رشد کند (مثال کلاسیک: naked short call). |
| **Max loss** | بدترین حالت در یک معاملهٔ defined-risk. Spruce اندازهٔ موقعیت را از این عدد می‌گیرد. |
| **Max profit** | در credit spread، تقریباً همان creditای که جمع کرده‌اید. |
| **Breakeven** | قیمت سهام در expiry که P&amp;L حدود صفر است (بدون کارمزد). |

## Greeks و واژه‌های پرتفوی

| Term | معنی ساده |
|------|----------------|
| **Delta** | حساسیت به حرکت \$1 سهام؛ همچنین یک heuristic تقریبی برای «شانس تمام‌شدن ITM». |
| **Theta** | Time decay. |
| **IV** | Implied volatility — بازاری چقدر حرکت را قیمت‌گذاری کرده. |
| **Buying power** | سرمایه‌ای که کارگزار برای معامله کنار می‌گذارد — با max loss یکی نیست. |
| **Heat** | مجموع max lossهای defined باز، در مقایسه با equity حساب. |
| **Roll** | بستن یک موقعیت و بازکردن strike/expiry مرتبط برای مدیریت ریسک یا زمان. |
| **CSP** | Cash-secured put — short put با پشتوانهٔ نقد برای assignment. |
| **Wheel** | چرخهٔ cash-secured put و covered call. موضوع بعدی. |
| **Covered call** | Short call روی سهامی که از قبل دارید. |
| **HITL** | Human-in-the-loop — پیشنهاد مجاز است؛ ارسال زنده به یک نفر نیاز دارد. |
| **Dry-run** | تمرین / آماده‌سازی بدون ارسال سفارش زنده. |

فرمول‌های payoff برای تک‌آپشن در [Payoffهای تک‌آپشن](single-option-payoffs.md) است. فرمول‌های credit spread در [Payoffهای credit spread](payoff-diagrams-credit-spreads.md) است. ساختارها را در [مقایسهٔ استراتژی‌ها](../04-portfolio-and-risk/comparing-strategies-example.md) مقایسه کنید. مراجع عمومی: [منابع](../00-meta/sources.md).
