# Manual Upwork Job Scraper

A working Selenium-based scraper that opens Upwork in a browser for manual verification, then extracts job data.

## Quick Start

1. **Install dependencies:**
   ```bash
   pip install selenium webdriver-manager
   ```

2. **Run the manual scraper:**
   ```bash
   python manual_upwork.py
   ```

3. **Follow the instructions:**
   - Browser will open to Upwork search page
   - Manually solve any verification/captcha
   - Wait for job listings to load (you have 20 seconds)
   - Scraper will automatically start extracting data
   - Browser stays open for 30 seconds after extraction

## Features

- ✅ Manual verification bypass (human-assisted)
- ✅ Extracts comprehensive job data
- ✅ Saves to CSV and JSON formats
- ✅ Prevents duplicate entries
- ✅ Works with Upwork's bot detection

## Data Extracted

For each job listing:
- Job title
- Description
- Budget/hourly rate
- Required skills
- Client information
- Posted time
- Job URL
- All available job details

## Output Files

- `manual_upwork_extraction_YYYYMMDD_HHMMSS.csv` - Spreadsheet format
- `manual_upwork_extraction_YYYYMMDD_HHMMSS.json` - JSON format

## Requirements

- Python 3.7+
- Chrome browser
- selenium
- webdriver-manager

## Legal Notice

⚠️ **Important**: Always respect Upwork's Terms of Service. This tool is for educational purposes. Use responsibly and don't overwhelm their servers.

## Troubleshooting

**Chrome driver issues**: The webdriver-manager handles this automatically.

**No jobs extracted**: Make sure jobs are loaded within the 20-second window.

**Browser closes too quickly**: The browser stays open for 30 seconds after extraction for manual review.

**Verification takes too long**: If you need more time, you can modify the 20-second delay in the code.
