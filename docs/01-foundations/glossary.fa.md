# Glossary

تعریف‌ها به زبان ساده. یک‌بار ورق بزنید؛ هر وقت صفحه‌ای اصطلاحی آورد که یادتان رفت، برگردید این‌جا.

خود اصطلاح‌ها English می‌مانند؛ توضیح‌شان فارسی است.

!!! danger "توصیه مالی نیست"
    فقط تعریف آموزشی.

## بلوک‌های اصلی

| Term | معنی ساده |
|------|----------------|
| **Call** | قرارداد با حق **خرید** سهام در strike. |
| **Put** | قرارداد با حق **فروش** سهام در strike. |
| **Premium** | قیمت option (یا net credit/debit یک معاملهٔ چندپا). |
| **Strike** | قیمتی که در قرارداد آمده. |
| **Expiration** | وقتی قرارداد تمام می‌شود. |
| **ITM** | In the money — call وقتی سهام بالای strike است؛ put وقتی سهام پایین strike است. |
| **OTM** | Out of the money — برعکس ITM. |
| **ATM** | At the money — سهام نزدیک strike. |

## Spreads و شکل ریسک

| Term | معنی ساده |
|------|----------------|
| **Credit spread** | معاملهٔ چندپا باز می‌کنید و **net credit** می‌گیرید. معمولاً یک short option، به‌علاوهٔ یک long option برای حفاظت. |
| **PCS / put credit spread** | یک put می‌فروشید و یک put پایین‌تر می‌خرید. به آن **bull put spread** هم می‌گویند. می‌خواهید سهام بالای short put بماند. |
| **CCS / call credit spread** | یک call می‌فروشید و یک call بالاتر می‌خرید. به آن **bear call spread** هم می‌گویند. می‌خواهید سهام زیر short call بماند. |
| **Defined risk** | بدترین زیان را از روی خود ساختار، همان موقع ورود، می‌دانید (قبل از کارمزد). |
| **Undefined risk** | زیان سقف تمیزی ندارد (مثال کلاسیک: naked short call). |
| **Max loss** | بدترین حالت در معاملهٔ defined-risk. Spruce اندازهٔ موقعیت را از همین عدد می‌گیرد. |
| **Max profit** | در credit spread، تقریباً همان creditای که گرفته‌اید. |
| **Breakeven** | قیمت سهام در expiry که P&amp;L حدود صفر است (بدون کارمزد). |

## Greeks و واژه‌های پرتفوی

| Term | معنی ساده |
|------|----------------|
| **Delta** | اگر سهام \$1 حرکت کند، قیمت option حدوداً چقدر عوض می‌شود؛ گاهی هم به‌عنوان تقریب «شانس تمام‌شدن ITM». |
| **Theta** | Time decay. |
| **IV** | Implied volatility — بازار چقدر حرکت را در قیمت گذاشته. |
| **Buying power** | پولی که کارگزار برای معامله کنار می‌گذارد — با max loss یکی نیست. |
| **Heat** | جمع max lossهای defined باز، نسبت به equity حساب. |
| **Roll** | بستن موقعیت و باز کردن strike یا expiry نزدیک، برای مدیریت ریسک یا زمان. |
| **CSP** | Cash-secured put — short put با نقد کنارگذاشته برای assignment. |
| **Wheel** | چرخهٔ cash-secured put و covered call. بعداً به آن می‌رسیم. |
| **Covered call** | Short call روی سهامی که از قبل دارید. |
| **HITL** | Human-in-the-loop — پیشنهاد آزاد است؛ ارسال سفارش زنده باید با خود آدم باشد. |
| **Dry-run** | تمرین و آماده‌سازی، بدون ارسال سفارش زنده. |

فرمول payoff تک‌آپشن در [Payoff تک‌آپشن](single-option-payoffs.md) است. فرمول credit spread در [Payoff مربوط به credit spread](payoff-diagrams-credit-spreads.md) است. ساختارها را در [مقایسهٔ استراتژی‌ها](../04-portfolio-and-risk/comparing-strategies-example.md) ببینید. مراجع عمومی: [منابع](../00-meta/sources.md).
