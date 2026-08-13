# Payoffهای credit spread

قبلاً دیدید که credit spreads **یکی** از ابزارهای defined-risk در میان چند ابزارند. این صفحه ریاضی و شکل فقط برای put و call credit spreads است.

!!! danger "توصیه مالی نیست"
    کارمزد، assignment زودهنگام، و margin کارگزار نتیجهٔ واقعی را عوض می‌کنند. اعداد کارمزد را نادیده می‌گیرند.

## یادآوری: چرا max loss اغلب از max profit بیشتر است

یک credit spread روی عرض \(W\) یک net credit برابر \(C\) جمع می‌کند. سپس:

\[
\text{Max profit} \approx C
\]

\[
\text{Max loss} \approx W - C
\]

هر وقت \(C &lt; W/2\)، max loss از max profit بزرگ‌تر است. این رایج است: شما یک ناحیهٔ با احتمال بالاتر را در ازای چک محدود می‌فروشید، و برای long optionای که فاجعه را سقف می‌گذارد **پول داده‌اید**. با debit spread در [صفحهٔ مقایسه](../04-portfolio-and-risk/comparing-strategies-example.md) مقایسه کنید، جایی که max profit می‌تواند از debit بیشتر شود.

---

## نمادهای مشترک

| Symbol | معنی |
|--------|---------|
| \(K_s\) | Short strike |
| \(K_l\) / \(K_h\) | Long put (پایین‌تر) / long call (بالاتر) |
| \(W\) | عرض بین strikeها |
| \(C\) | Net credit به‌ازای سهم |

برای قرارداد سهام استاندارد در ۱۰۰ ضرب کنید.

---

## Put credit spread (bull put)

Put برابر \(K_s\) را بفروشید، put برابر \(K_l\) را بخرید، همان expiry. \(W = K_s - K_l\).

| Outcome | Formula |
|---------|---------|
| Max profit | \(C\) اگر سهام ≥ \(K_s\) |
| Max loss | \(W - C\) اگر سهام ≤ \(K_l\) |
| Breakeven | \(K_s - C\) |

<figure markdown="span">
  <svg viewBox="0 0 520 260" width="100%" role="img" aria-label="Put credit spread payoff">
    <line x1="60" y1="20" x2="60" y2="220" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="60" y1="120" x2="500" y2="120" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="80,200 180,200 300,120 360,50 480,50"/>
    <text x="50" y="54" text-anchor="end" font-size="12" fill="currentColor">+C</text>
    <text x="50" y="124" text-anchor="end" font-size="12" fill="currentColor">0</text>
    <text x="50" y="204" text-anchor="end" font-size="12" fill="currentColor">-(W−C)</text>
    <text x="180" y="240" text-anchor="middle" font-size="12" fill="currentColor">Kl</text>
    <text x="300" y="240" text-anchor="middle" font-size="12" fill="currentColor">BE</text>
    <text x="360" y="240" text-anchor="middle" font-size="12" fill="currentColor">Ks</text>
    <text x="480" y="240" text-anchor="middle" font-size="12" fill="currentColor">price →</text>
  </svg>
</figure>

### مثال با credit سالم‌تر (باز هم زیان &gt; سود)

Spread put برابر \$100 / \$95 را به credit **\$2.00** بفروشید (\$200).

- Max profit = **\$200**  
- Max loss = **\$300**  
- Breakeven = \$98  

پایان صعودی (سهام \$110): **+\$200**. پایان نزولی از \$95 عبور کند: **−\$300**.  
Credit را نسبت به مثال لاغر \$1.50 بهتر کردید، اما ساختار همچنان پاداش محدود در ازای زیان defined بزرگ‌تر می‌پردازد — از روی طراحی.

---

## Call credit spread (bear call)

Call برابر \(K_s\) را بفروشید، call برابر \(K_h\) را بخرید. \(W = K_h - K_s\). Breakeven برابر \(K_s + C\).

<figure markdown="span">
  <svg viewBox="0 0 520 260" width="100%" role="img" aria-label="Call credit spread payoff">
    <line x1="60" y1="20" x2="60" y2="220" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="60" y1="120" x2="500" y2="120" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="80,50 200,50 260,120 380,200 480,200"/>
    <text x="50" y="54" text-anchor="end" font-size="12" fill="currentColor">+C</text>
    <text x="50" y="124" text-anchor="end" font-size="12" fill="currentColor">0</text>
    <text x="50" y="204" text-anchor="end" font-size="12" fill="currentColor">-(W−C)</text>
    <text x="200" y="240" text-anchor="middle" font-size="12" fill="currentColor">Ks</text>
    <text x="260" y="240" text-anchor="middle" font-size="12" fill="currentColor">BE</text>
    <text x="380" y="240" text-anchor="middle" font-size="12" fill="currentColor">Kh</text>
    <text x="480" y="240" text-anchor="middle" font-size="12" fill="currentColor">price →</text>
  </svg>
</figure>

### مثال

Spread call برابر \$100 / \$105 را به credit **\$1.80** بفروشید.

- Max profit = **\$180**  
- Max loss = **\$320**  
- Breakeven = \$101.80  

---

## عادت‌ها

1. اندازه را از max loss برابر \(W - C\) بگیرید، نه از قیمت سهم.  
2. Defined به‌معنای کوچک نیست.  
3. وقتی کف مشخص می‌خواهید، این ساختار را به naked short ترجیح دهید.  
4. اگر از «زیان بزرگ‌تر از سود» خوشتان نمی‌آید، شاید debit spreads یا long options برای آن ایده مناسب‌تر باشند — [مقایسه](../04-portfolio-and-risk/comparing-strategies-example.md) را دوباره ببینید.

## گام بعدی

[Defined-risk credit spreads](../03-strategies/defined-risk-credit-spreads.md) · [Playbook مربوط به PCS](../03-strategies/put-credit-spread-playbook.md) · [Playbook مربوط به CCS](../03-strategies/call-credit-spread-playbook.md)

## منابع

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان راستی‌آزمایی کنید.*
