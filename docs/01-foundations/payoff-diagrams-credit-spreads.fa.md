# Payoff مربوط به credit spread

قبلاً دیدید credit spread **یکی** از چند ابزار defined-risk است. این صفحه فقط ریاضی و شکل put و call credit spread است.

!!! danger "توصیه مالی نیست"
    کارمزد، assignment زودهنگام، و margin کارگزار نتیجهٔ واقعی را عوض می‌کنند. عددها کارمزد ندارند.

## یادآوری: چرا max loss معمولاً از max profit بیشتر است

یک credit spread روی عرض \(W\)، net credit برابر \(C\) می‌گیرد. بعد:

\[
\text{Max profit} \approx C
\]

\[
\text{Max loss} \approx W - C
\]

هر وقت \(C &lt; W/2\)، max loss از max profit بزرگ‌تر است. این رایج است: ناحیه‌ای با احتمال بالاتر را در ازای یک چک محدود می‌فروشید، و برای long optionای که فاجعه را سقف می‌گذارد **پول داده‌اید**. با debit spread در [صفحهٔ مقایسه](../04-portfolio-and-risk/comparing-strategies-example.md) بسنجید؛ آن‌جا max profit می‌تواند از debit بیشتر شود.

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

Put در \(K_s\) بفروشید، put در \(K_l\) بخرید، همان expiry. \(W = K_s - K_l\).

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

### مثال با credit بهتر (باز هم زیان &gt; سود)

Spread put برابر \$100 / \$95 را با credit **\$2.00** باز کنید (\$200).

- Max profit = **\$200**  
- Max loss = **\$300**  
- Breakeven = \$98  

اگر سهام \$110 تمام شود: **+\$200**. اگر از \$95 رد شود: **−\$300**.  
Credit از مثال لاغر \$1.50 بهتر شد، ولی ساختار هنوز پاداش محدود می‌دهد در ازای زیان defined بزرگ‌تر — از روی طراحی.

---

## Call credit spread (bear call)

Call در \(K_s\) بفروشید، call در \(K_h\) بخرید. \(W = K_h - K_s\). Breakeven برابر \(K_s + C\).

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

Spread call برابر \$100 / \$105 را با credit **\$1.80** باز کنید.

- Max profit = **\$180**  
- Max loss = **\$320**  
- Breakeven = \$101.80  

---

## عادت‌ها

1. اندازه را از max loss برابر \(W - C\) بگیرید، نه از قیمت سهم.  
2. Defined یعنی کوچک نیست.  
3. اگر کف مشخص می‌خواهید، این ساختار را به naked short ترجیح دهید.  
4. اگر از «زیان بزرگ‌تر از سود» خوشتان نمی‌آید، شاید debit spread یا long option برای آن ایده مناسب‌تر باشد — [مقایسه](../04-portfolio-and-risk/comparing-strategies-example.md) را دوباره ببینید.

## بعد چه بخوانید

[Defined-risk credit spreads](../03-strategies/defined-risk-credit-spreads.md) · [Playbook مربوط به PCS](../03-strategies/put-credit-spread-playbook.md) · [Playbook مربوط به CCS](../03-strategies/call-credit-spread-playbook.md)

## منابع

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [فهرست منابع](../00-meta/sources.md)  

---

*توصیه مالی نیست. قوانین کارگزار را خودتان چک کنید.*
