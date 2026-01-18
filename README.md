# French Tech Funding Wire Infographic

Interactive infographic templates for visualizing French startup funding data.

## Files

### Annual Report
- **report.html** - Annual funding report (e.g., 2025 Year in Review)
- **funding-data.json** - Full year funding data

### Weekly Newsletter
- **weekly-report.html** - Weekly funding snapshot for newsletter
- **weekly-data.json** - Weekly funding data (last 7 days)

## Data Format

Both templates use the same JSON data structure:

```json
[
  {
    "company": "Company Name",
    "amount": 468,
    "sectors": ["AI & Machine Learning", "DeepTech & Hardware"],
    "date": "2025-01-15"
  }
]
```

### Fields

- **company** (required): Company name
- **amount** (required): Funding amount in millions of euros (e.g., 468 = €468M)
- **sectors** (optional): Array of sector tags
- **date** (optional for annual, required for weekly): ISO date format (YYYY-MM-DD)

### Available Sectors

- AI & Machine Learning
- HealthTech & BioTech
- CleanTech & Energy
- FinTech
- Gaming
- DeepTech & Hardware
- SpaceTech & Aerospace
- AgriTech & FoodTech
- SaaS & Enterprise
- E-commerce & Retail
- Mobility & Transportation
- Cybersecurity
- PropTech & Real Estate
- Other

## Using the Weekly Template

1. **Prepare your data**: Create/update `weekly-data.json` with the week's funding deals
2. **Open the report**: Open `weekly-report.html` in a browser
3. **The template will**:
   - Calculate total funding and deal count
   - Show top deals ranked by amount
   - Display sector breakdown with interactive toggles
   - Auto-calculate the date range from your data

### Weekly Data Tips

- Include all deals from the past 7 days
- The date range will auto-calculate from the earliest and latest dates in your data
- You can include deals without amounts (they'll be counted but won't affect funding totals)
- Multiple sectors per company are supported

## Using the Annual Report

1. **Prepare your data**: Create/update `funding-data.json` with the full year's deals
2. **Open the report**: Open `report.html` in a browser
3. **Features**:
   - Annual totals and statistics
   - Top 10 deals of the year
   - Comprehensive sector analysis
   - Interactive funding/company count toggle

## Customization

Both templates use the same color scheme and sector colors. To customize:

- **Colors**: Edit the `sectorColors` object in the JavaScript section
- **Layout**: Modify the CSS in the `<style>` section
- **Stats displayed**: Edit the JavaScript `renderAll()` function

## Browser Compatibility

These templates work in all modern browsers. No build process or dependencies required - just open the HTML files directly.
