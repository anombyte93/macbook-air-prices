# MacBook Air Price Research - Data Collection Notes

## Completed Tasks
- ✓ Created structured JSON template with all 5 retailers
- ✓ Identified URLs for each retailer
- ✓ Set up baseline pricing data (M3: $1,549-$1,599 | M2: $1,199-$1,299)
- ✓ Configured data structure for delivery, promotions, and stock status

## Data File Structure
```json
{
  "timestamp": "ISO 8601 date",
  "currency": "AUD",
  "location": "Perth, WA",
  "retailers": {
    "retailer_key": {
      "name": "Retailer Name",
      "url": "retailer_url",
      "models": {
        "m3_13": { "price_aud": 1549, "in_stock": null },
        "m2_13": { "price_aud": 1199, "in_stock": null }
      },
      "promotions": [],
      "delivery_to_perth": { "available": true, "estimated_days": null }
    }
  }
}
```

## Retailers Included
| Retailer | Status | URL |
|----------|--------|-----|
| Apple Store AU | Template | https://www.apple.com/au/shop/buy-mac/macbook-air |
| JB Hi-Fi | Template | https://www.jbhifi.com.au/products/apple-macbook-air-13-m3 |
| Harvey Norman | Template | https://www.harveynorman.com.au/computers/apple-macbook |
| Officeworks | Template | https://www.officeworks.com.au/search?q=MacBook+Air |
| The Good Guys | Template | https://www.thegoodguys.com.au/apple/laptops/macbook-air |

## Next Steps for Live Verification
1. Use browser automation to scrape current prices
2. Extract active promotions (holiday sales, bundle deals)
3. Verify Perth delivery availability and costs
4. Check stock status for each model
5. Generate comparative pricing report
