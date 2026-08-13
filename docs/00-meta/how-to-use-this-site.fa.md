# نحوه استفاده از این سایت

Spruce یک دورهٔ کوتاه است. وسوسهٔ پریدن مستقیم به playbookهای credit spread را کنار بگذارید. آن صفحات فرض می‌کنند options و منوی ریسک را از قبل می‌فهمید.

!!! danger "توصیه مالی نیست"
    فقط محتوای آموزشی. قوانین کارگزار و CRA را خودتان راستی‌آزمایی کنید.

## مسیر مطالعه

**بخش A — مکانیک**

1. [سلب مسئولیت](disclaimer.md)  
2. [Glossary](../01-foundations/glossary.md)  
3. [مبانی آپشن](../01-foundations/options-basics.md)  
4. [Payoffهای تک‌آپشن](../01-foundations/single-option-payoffs.md)  
5. [Greeks](../01-foundations/greeks-enough-to-operate.md) → [Weekly در برابر monthly](../01-foundations/expirations-weekly-monthly.md)  

**بخش B — مدیریت ریسک**

6. [روش‌های مدیریت ریسک](../04-portfolio-and-risk/risk-management-categories.md)  
7. [مقایسهٔ استراتژی‌ها با یک مثال](../04-portfolio-and-risk/comparing-strategies-example.md)  

**بخش C — Credit spreads (یک ابزار)**

8. [Payoffهای credit spread](../01-foundations/payoff-diagrams-credit-spreads.md)  
9. Playbookها و [سیاست ریسک](../04-portfolio-and-risk/risk-policy.md)  
10. یادداشت‌های کانادایی در صورت مرتبط بودن  

## برچسب‌ها

| Tag | معنی |
|-----|---------|
| `[verified]` | با منابع عمومی مستقل یا صفحهٔ اصلی کارگزار هم‌خوان است |
| `[operator preference]` | پیش‌فرض آموزشی که می‌توانید تغییر دهید |
| `[pending-verify]` | به منبع اولیهٔ قوی‌تری نیاز دارد |

## پیش‌نمایش محلی

```bash
pip install -r requirements.txt
mkdocs serve -f mkdocs.public.yml   # public site
mkdocs serve                        # includes private operator pages
```
