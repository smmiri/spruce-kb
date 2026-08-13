# Payoff تک‌آپشن

چهار تصویر، هر کدام یک ایده. هنوز خبری از spread نیست — فقط اگر تا expiration نگه دارید، بر سر P&amp;L چه می‌آید (کارمزد را حساب نکرده‌ایم).

!!! danger "توصیه مالی نیست"
    فقط آموزش است. Assignment زودهنگام و کارمزد نتیجهٔ واقعی را عوض می‌کنند.

## فرض مشترک مثال‌ها

فرض کنید سهام **XYZ** نزدیک \$100 است. یک قرارداد = ۱۰۰ سهم. Premiumهای زیر به‌ازای هر سهم‌اند؛ برای دلار هر قرارداد در ۱۰۰ ضرب کنید.

---

## ۱. Long call — برای بالا رفتن سهام پول داده‌اید

Call با strike برابر \$100 را به \$3.00 می‌خرید (\$300 به‌ازای قرارداد).

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

**مثال سود:** سهام روی \$110 تمام می‌شود → call حدود \$10 می‌ارزد → سود ≈ \$7 در هر سهم (\$700).  
**مثال زیان:** سهام روی \$95 تمام می‌شود → call بی‌ارزش expire می‌شود → همان \$300 premium از دست می‌رود.

---

## ۲. Long put — برای پایین آمدن سهام پول داده‌اید

Put با strike برابر \$100 را به \$2.50 می‌خرید (\$250).

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

**مثال سود:** سهام روی \$85 تمام می‌شود → put حدود \$15 می‌ارزد → سود ≈ \$12.50 در هر سهم.  
**مثال زیان:** سهام روی \$105 تمام می‌شود → put بی‌ارزش → \$250 از دست می‌رود.

---

## ۳. Short call — premium گرفته‌اید (naked)

Call با strike برابر \$100 را به \$3.00 می‌فروشید و سهام **ندارید**.

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

**مثال سود:** سهام روی \$90 تمام می‌شود → call بی‌ارزش expire می‌شود → \$300 می‌ماند.  
**مثال زیان:** سهام روی \$130 تمام می‌شود → short call حدود \$27 در هر سهم زیان می‌دهد، قبل از کم کردن credit برابر \$3 → حدود \$2,400 به‌ازای قرارداد. سهام هنوز می‌تواند بالاتر برود. `[verified]` برای uncovered call، ریسک صعود سقف ندارد.

---

## ۴. Short put — premium گرفته‌اید (naked / هنوز cash-secured نیست)

Put با strike برابر \$100 را به \$2.50 می‌فروشید.

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

**مثال سود:** سهام روی \$110 تمام می‌شود → put بی‌ارزش → \$250 می‌ماند.  
**مثال زیان:** سهام روی \$70 تمام می‌شود → زیان ≈ \$27.50 در هر سهم (\$2,750) بعد از credit.

---

## این چهار تا چه می‌گویند

1. خریدار زیان **محدود** دارد (همان premium) و به حرکت نیاز دارد.  
2. فروشندهٔ naked سود **محدود** دارد (همان premium) و ممکن است با زیان **خیلی بزرگ‌تر** روبه‌رو شود.  
3. باگ فرمول نیست — وقتی بدون hedge بیمه می‌فروشید، همین معامله را پذیرفته‌اید.

موضوع بعدی «یک credit spread انتخاب کنید» نیست. این است: **چه دسته‌هایی از مدیریت ریسک هست**، و سود و زیان‌شان روی همان داستان سهام چطور فرق می‌کند.

بعد بروید سراغ [Greeks](greeks-enough-to-operate.md)، بعد [راه‌های مدیریت ریسک](../04-portfolio-and-risk/risk-management-categories.md).

## منابع

- OCC *Characteristics and Risks of Standardized Options*  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان چک کنید.*
