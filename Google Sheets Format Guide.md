# Google Sheets Format for WMSU Palaro Scoreboard

## Required Sheet Structure

Your Google Sheet should have the following columns in **Sheet1**:

| Column | Letter | Field Name | Description | Example |
|--------|--------|------------|-------------|---------|
| 1 | A | Team 1 Name | First team's name | "Engineering" |
| 2 | B | Team 1 Score | First team's current score | "15" |
| 3 | C | Team 1 Logo | Emoji or symbol for team 1 | "🔧" |
| 4 | D | Team 1 Color | Hex color code for team 1 | "#3498db" |
| 5 | E | Team 2 Name | Second team's name | "Business" |
| 6 | F | Team 2 Score | Second team's current score | "12" |
| 7 | G | Team 2 Logo | Emoji or symbol for team 2 | "💼" |
| 8 | H | Team 2 Color | Hex color code for team 2 | "#e74c3c" |
| 9 | I | Sport Name | Name of the sport | "Basketball" |
| 10 | J | Sport Icon | Emoji for the sport | "🏀" |
| 11 | K | Game Type | Type of match | "Finals" |
| 12 | L | Status | Current game status | "LIVE" or "In Progress" |

## Sample Data Format

Here's how your data should look in the spreadsheet:

```
Team 1 Name | Team 1 Score | Team 1 Logo | Team 1 Color | Team 2 Name | Team 2 Score | Team 2 Logo | Team 2 Color | Sport Name | Sport Icon | Game Type | Status
Engineering | 15 | 🔧 | #3498db | Business | 12 | 💼 | #e74c3c | Basketball | 🏀 | Finals | LIVE
Computer Science | 8 | 💻 | #2ecc71 | Education | 6 | 📚 | #f39c12 | Volleyball | 🏐 | Semifinals | In Progress
Nursing | 21 | 🩺 | #9b59b6 | Medicine | 18 | ⚕️ | #1abc9c | Football | ⚽ | Quarterfinals | LIVE
```

## Important Notes

1. **Header Row**: The first row (Row 1) should contain headers, but the code reads from Row 2 onwards
2. **Empty Cells**: Use empty strings for missing data, not null values
3. **Status Values**: Use "LIVE" for live games (shows pulsing red dot), any other text for non-live games
4. **Color Format**: Use hex color codes (e.g., #3498db) for team colors
5. **Emojis**: Use emoji characters for logos and sport icons

## Setting Up Your Google Sheet

1. Create a new Google Sheet
2. Name the first sheet "Sheet1"
3. Add the headers in Row 1 (optional, but recommended)
4. Add your game data starting from Row 2
5. Make sure the sheet is publicly accessible or shared with the API key
6. Copy the Sheet ID from the URL (the long string between `/d/` and `/edit`)

## Example URL Structure
```
https://docs.google.com/spreadsheets/d/1EJfto3fshSHuYLUwWLCb7JaDmFKQdXJlunMlyNOwYx8/edit
```
Sheet ID: `1EJfto3fshSHuYLUwWLCb7JaDmFKQdXJlunMlyNOwYx8`

## Troubleshooting

- **No data showing**: Check if your sheet has data in the correct columns
- **Wrong data displayed**: Verify column order matches the expected format
- **Connection errors**: Ensure the sheet is publicly accessible
- **Missing games**: Check if there are empty rows or missing required columns
