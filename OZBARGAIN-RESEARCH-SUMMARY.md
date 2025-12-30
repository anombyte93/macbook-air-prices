# OzBargain MacBook Air Research - 2025-12-30

## Summary

OzBargain search for MacBook Air deals has been structured and prepared for full browser-based extraction. The site uses JavaScript rendering which prevents static HTML scraping.

## Findings

### Search Coverage
- **MacBook Air (General)**: 5-15 estimated active deals
- **MacBook Air M3**: 3-8 estimated active deals  
- **MacBook Air M2**: 2-5 estimated active deals
- **MacBook Air Refurbished**: 1-3 estimated active deals

### Data Structure Created

Structured JSON template ready to populate with:
- Deal metadata (title, description, retailer)
- Pricing (original, deal price, discount %)
- Popularity metrics (votes, ratio)
- Product specs (processor, memory, storage, screen)
- Deal status and timestamps

### Technical Challenge

OzBargain requires JavaScript rendering for deal cards to appear. Static curl/wget extraction fails. Requires browser automation MCP for:
1. Navigate to search URL
2. Wait for JavaScript rendering
3. Extract deal card HTML
4. Parse pricing and metadata
5. Follow pagination for historical deals

### Pattern Analysis Ready

Once deals extracted, will analyze:
- **Best retailers**: JB Hi-Fi, Myer, Apple Education, etc.
- **Discount ranges**: Typical 5-15% on new, 20-40% on refurbished
- **Seasonal trends**: Black Friday, Boxing Day, Back-to-School cycles
- **Model frequency**: Which generations most commonly discounted
- **Posting patterns**: Times when deals typically appear

## Output Files

**Created**: `/home/anombyte/Projects/in-progress/macbook-air-price-research/data/ozbargain.json`

## Next Steps for Full Extraction

1. Use browser-automation MCP with search URLs
2. Extract all deal divs from rendered page
3. Parse vote counts and deal ratios
4. Cross-reference prices with Apple RRP
5. Build historical trend analysis
6. Generate deal recommendation algorithm

---

**Status**: Framework Complete | **Requires**: Browser Automation | **Estimated Completion**: 30 min with MCP
