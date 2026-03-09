Polymarket Edge Scanner
Live Black-Scholes edge scanner for Polymarket prediction markets.
URL
https://avivso.github.io/Polymarket-scanner-4

What it does

Fetches the top 300 Polymarket markets by volume, prices each one using Black-Scholes, and ranks them by edge — the gap between theoretical fair value and current market price.
Hit RESCAN anytime to refresh all prices live.
Signals
	∙	⚡ HARD YES — BS fair value > market price by 15%+ → BET YES
	∙	↑ YES — BS fair value > market price by 6–15% → BET YES
	∙	— NEUTRAL — within 6% either way
	∙	↓ NO — market overprices YES by 6–15% → BET NO
	∙	⚡ HARD NO — market overprices YES by 15%+ → BET NO
Formula
V = e^(-rT) × N(d₂) — K=0.5, r=5%, σ auto-estimated by category
Disclaimer
Not financial advice.​​​​​​​​​​​​​​​​
