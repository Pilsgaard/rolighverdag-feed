# Rolig Hverdag – Partner-ads-feed

Kopi af produktfeedet fra rolighverdag.dk, så Partner-ads kan hente det uden om Shopifys bot-beskyttelse.

- **Feed-URL til Partner-ads:** https://raw.githubusercontent.com/Pilsgaard/rolighverdag-feed/main/partnerads.xml
- **Kilde:** https://rolighverdag.dk/collections/AffiliatePartnerAds?view=xml (skabelonen `collection.xml.liquid` i temaet)
- **Opdatering:** GitHub Actions kører hver morgen og ved klik på *Actions → Opdater Partner-ads-feed → Run workflow*.

Jobbet tjekker, at feedet er gyldig XML med mindst ét produkt. Ellers fejler det (GitHub sender en mail), og den sidste gode version bliver liggende.
