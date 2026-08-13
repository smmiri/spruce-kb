# Payoffهای تک‌آپشن

چهار تصویر. هر کدام یک ایده. هنوز spread نیست — فقط چه بر سر P&amp;L می‌آید اگر تا expiration نگه دارید (کارمزد نادیده گرفته شده).

!!! danger "توصیه مالی نیست"
    فقط محتوای آموزشی. Assignment زودهنگام و کارمزد نتیجهٔ واقعی را عوض می‌کنند.

## تنظیم مشترک مثال‌ها

فرض کنید سهام **XYZ** نزدیک \$100 است. یک قرارداد = ۱۰۰ سهم. Premiumهای زیر به‌ازای هر سهم هستند؛ برای دلار به‌ازای قرارداد در ۱۰۰ ضرب کنید.

---

## ۱. Long call — برای صعود پول داده‌اید

Call برابر \$100 را به \$3.00 می‌خرید (\$300 به‌ازای قرارداد).

\[
\text{Max loss} = \text{premium paid} = \$3
\]

\[
\text{Breakeven} = \text{strike} + \text{premium} = \$103
\]

\[
\text{Max profit} = \text{unlimited in theory as the stock rises}
\]

<figure markdown="span">
  <svg viewBox="0 0 520 240" width="100%" role="img" aria-label="Long call payoff">
    <line x1="50" y1="20" x2="50" y2="200" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="50" y1="140" x2="490" y2="140" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="70,170 220,170 280,140 470,40"/>
    <text x="40" y="174" text-anchor="end" font-size="11" fill="currentColor">−prem</text>
    <text x="40" y="144" text-anchor="end" font-size="11" fill="currentColor">0</text>
    <text x="220" y="220" text-anchor="middle" font-size="11" fill="currentColor">K</text>
    <text x="280" y="220" text-anchor="middle" font-size="11" fill="currentColor">BE</text>
    <text x="460" y="220" text-anchor="middle" font-size="11" fill="currentColor">price →</text>
    <text x="270" y="16" text-anchor="middle" font-size="13" fill="currentColor">Long call at expiration</text>
  </svg>
</figure>

**مثال سود:** سهام \$110 تمام می‌شود → call حدود \$10 می‌ارزد → سود ≈ \$7/سهم (\$700).  
**مثال زیان:** سهام \$95 تمام می‌شود → call بی‌ارزش expire می‌شود → premium برابر \$300 از دست می‌رود.

---

## ۲. Long put — برای نزول پول داده‌اید

Put برابر \$100 را به \$2.50 می‌خرید (\$250).

\[
\text{Max loss} = \text{premium paid}
\]

\[
\text{Breakeven} = \text{strike} - \text{premium} = \$97.50
\]

\[
\text{Max profit} \approx \text{strike} - \text{premium (if stock goes to zero)}
\]

<figure markdown="span">
  <svg viewBox="0 0 520 240" width="100%" role="img" aria-label="Long put payoff">
    <line x1="50" y1="20" x2="50" y2="200" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="50" y1="140" x2="490" y2="140" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="70,40 200,140 260,170 470,170"/>
    <text x="40" y="174" text-anchor="end" font-size="11" fill="currentColor">−prem</text>
    <text x="40" y="144" text-anchor="end" font-size="11" fill="currentColor">0</text>
    <text x="200" y="220" text-anchor="middle" font-size="11" fill="currentColor">BE</text>
    <text x="260" y="220" text-anchor="middle" font-size="11" fill="currentColor">K</text>
    <text x="460" y="220" text-anchor="middle" font-size="11" fill="currentColor">price →</text>
    <text x="270" y="16" text-anchor="middle" font-size="13" fill="currentColor">Long put at expiration</text>
  </svg>
</figure>

**مثال سود:** سهام \$85 تمام می‌شود → put حدود \$15 می‌ارزد → سود ≈ \$12.50/سهم.  
**مثال زیان:** سهام \$105 تمام می‌شود → put بی‌ارزش → \$250 از دست می‌رود.

---

## ۳. Short call — premium جمع کرده‌اید (naked)

Call برابر \$100 را به \$3.00 می‌فروشید و سهام **ندارید**.

\[
\text{Max profit} = \text{premium received} = \$3
\]

\[
\text{Breakeven} = \$103
\]

\[
\text{Max loss} = \text{theoretically unlimited if the stock rises}
\]

<figure markdown="span">
  <svg viewBox="0 0 520 240" width="100%" role="img" aria-label="Short call naked payoff">
    <line x1="50" y1="20" x2="50" y2="200" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="50" y1="100" x2="490" y2="100" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="70,70 220,70 280,100 470,200"/>
    <text x="40" y="74" text-anchor="end" font-size="11" fill="currentColor">+prem</text>
    <text x="40" y="104" text-anchor="end" font-size="11" fill="currentColor">0</text>
    <text x="220" y="220" text-anchor="middle" font-size="11" fill="currentColor">K</text>
    <text x="280" y="220" text-anchor="middle" font-size="11" fill="currentColor">BE</text>
    <text x="460" y="220" text-anchor="middle" font-size="11" fill="currentColor">price →</text>
    <text x="270" y="16" text-anchor="middle" font-size="13" fill="currentColor">Naked short call at expiration</text>
  </svg>
</figure>

**مثال سود:** سهام \$90 تمام می‌شود → call بی‌ارزش expire می‌شود → \$300 می‌ماند.  
**مثال زیان:** سهام \$130 تمام می‌شود → short call حدود \$27/سهم قبل از احتساب credit برابر \$3 زیان می‌دهد → حدود \$2,400 به‌ازای قرارداد. سهام هنوز می‌تواند بالاتر برود. `[verified]` ریسک صعود نامحدود برای uncovered callها.

---

## ۴. Short put — premium جمع کرده‌اید (naked / هنوز cash-secured نیست)

Put برابر \$100 را به \$2.50 می‌فروشید.

\[
\text{Max profit} = \text{premium received}
\]

\[
\text{Breakeven} = \$97.50
\]

\[
\text{Max loss} \approx \text{strike} - \text{premium (if stock → 0)}
\]

<figure markdown="span">
  <svg viewBox="0 0 520 240" width="100%" role="img" aria-label="Short put payoff">
    <line x1="50" y1="20" x2="50" y2="200" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="50" y1="100" x2="490" y2="100" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="70,200 200,100 260,70 470,70"/>
    <text x="40" y="74" text-anchor="end" font-size="11" fill="currentColor">+prem</text>
    <text x="40" y="104" text-anchor="end" font-size="11" fill="currentColor">0</text>
    <text x="200" y="220" text-anchor="middle" font-size="11" fill="currentColor">BE</text>
    <text x="260" y="220" text-anchor="middle" font-size="11" fill="currentColor">K</text>
    <text x="460" y="220" text-anchor="middle" font-size="11" fill="currentColor">price →</text>
    <text x="270" y="16" text-anchor="middle" font-size="13" fill="currentColor">Short put at expiration</text>
  </svg>
</figure>

**مثال سود:** سهام \$110 تمام می‌شود → put بی‌ارزش → \$250 می‌ماند.  
**مثال زیان:** سهام \$70 تمام می‌شود → زیان ≈ \$27.50/سهم (\$2,750) بعد از credit.

---

## این چهار تا چه می‌آموزند

1. خریداران زیان **محدود** دارند (همان premium) و به حرکت نیاز دارند.  
2. فروشندگان naked سود **محدود** دارند (همان premium) و می‌توانند با زیان **خیلی بزرگ‌تر** روبه‌رو شوند.  
3. این باگ فرمول نیست — معامله‌ای است که وقتی بیمه می‌فروشید بدون hedge می‌پذیرید.

موضوع بزرگ بعدی «یک credit spread انتخاب کنید» نیست. این است: **چه دسته‌هایی از مدیریت ریسک وجود دارد**، و پروفایل سود/زیان‌شان روی همان داستان سهام چگونه مقایسه می‌شود.

ادامه دهید به [Greeks](greeks-enough-to-operate.md)، سپس [روش‌های مدیریت ریسک](../04-portfolio-and-risk/risk-management-categories.md).

## منابع

- OCC *Characteristics and Risks of Standardized Options*  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان راستی‌آزمایی کنید.*
