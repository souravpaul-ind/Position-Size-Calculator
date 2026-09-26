# 📐 Position Size Calculator

A beautiful, lightweight, and fast position size calculator for crypto traders. Built with pure HTML, CSS, and JavaScript — no dependencies, no build step.

![Status](https://img.shields.io/badge/status-active-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Size](https://img.shields.io/badge/size-~30KB-blueviolet)

---

## ✨ Features

- 🎯 **Precise lot sizing** — calculates exact position size based on risk
- 📉 **Pips / Price SL modes** — choose how you enter your stop-loss
- 📦 **Coins / Lots units** — view position in coins or lots
- 🪙 **Multi-coin support** — BTC, ETH, XAUT, or Custom
- 📈 **Long / Short direction** — auto-validates SL placement
- ⚡ **Leverage cap** — never exceeds your max buying power
- 💎 **Glassmorphism UI** — modern semi-transparent design
- 🚀 **Optimized** — smooth on low-end devices
- 📱 **Fully responsive** — works on mobile & desktop

---

## 🚀 Live Demo

👉 **[Try it here](https://souravpaul-ind.github.io/position-size-calculator/)**

---

## 🛠️ How to Use

1. Open `index.html` in any browser (or visit the live demo)
2. Select your **Coin** (BTC / ETH / XAUT / Custom)
3. Choose **Direction** (Long / Short)
4. Select **Unit** (Coins / Lots)
5. Choose **SL Mode** (Pips / Price)
6. Enter:
   - **Capital** (your account size in USD)
   - **Risk %** (how much you're willing to lose)
   - **Leverage** (only for Price mode)
   - **SL** (either in pips or price)
   - **Lot Size** (minimum tradable amount per exchange)
7. Read your **Adjusted Position**, **Notional Value**, **Margin**, and **Max Loss**

---

## 🧮 Formulas Used

### Pips Mode

Max Loss ($) = Capital × Risk%
Position (coins) = Max Loss ÷ (Pips × 1) [1 pip = $1 per coin]
Lots = floor(Position ÷ Lot Size)

### Price Mode

Max Loss ($) = Capital × Risk%
Price Risk = |Entry − Stop|
Risk-based Size = Max Loss ÷ Price Risk
Leverage Cap = (Capital × Leverage) ÷ Entry
Ideal Size = min(Risk-based, Leverage Cap)
Lots = floor(Ideal Size ÷ Lot Size)
Notional Value = Lots × Lot Size × Entry
Margin Required = Notional ÷ Leverage
Actual Risk % = (Lots × Lot Size × Price Risk) ÷ Capital × 100


---

## 🧩 Tech Stack

- **HTML5**
- **CSS3** (Glassmorphism, animations, responsive)
- **Vanilla JavaScript** (no libraries, no frameworks)

---

## 📱 Browser Support

| Browser | Support |
|---------|---------|
| Chrome  | ✅ |
| Firefox | ✅ |
| Safari  | ✅ |
| Edge    | ✅ |
| Mobile  | ✅ |

---

## 📄 License

This project is licensed under the **MIT License**.

---

## ⚠️ Disclaimer

This tool is for **educational purposes only**. It does not constitute financial advice. Trading cryptocurrencies involves substantial risk of loss. Always do your own research and never trade more than you can afford to lose.

---

## ⭐ Show Your Support

If this helped you, please give it a ⭐ on GitHub!
