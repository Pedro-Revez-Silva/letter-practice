# Letter Practice Sheet Generator

A simple web application for generating printable letter practice sheets for children learning to write. Designed specifically for Portuguese manuscript handwriting but works with any Google Font.

## Why This Project?

I needed practice sheets for my daughter to learn Portuguese manuscript letters, but couldn't find any online with the specific letters drawn the way she needs to learn them. So I built this generator to create custom practice sheets using Google Fonts that support Portuguese manuscript writing (like "Playwrite PT Guides").

## Features

- **Custom Letter Selection**: Choose individual letters from A-Z
- **Letter Case Control**:
  - Show both uppercase and lowercase (default)
  - Uppercase only
  - Lowercase only
- **Letter Combinations**: Add custom letter combinations (e.g., "ai", "ui", "eu", "ão")
- **Google Fonts Support**: Use any Google Font (optimized for handwriting fonts with guide lines)
- **Print-Ready Output**: Generates HTML pages optimized for A4 printing
- **Guide Lines**: Automatically uses the font's built-in guide lines for proper letter formation

## How to Use

1. **Open `index.html`** in your web browser
2. **Enter a Google Font name** (e.g., "Playwrite PT Guides", "Playwrite PT", "Caveat")
3. **Select letters** to practice:
   - Click individual letters
   - Use "Todas" (All), "Vogais" (Vowels), or "Limpar" (Clear) buttons
4. **Choose case options** (optional):
   - Toggle "Apenas Maiúsculas" for uppercase only
   - Toggle "Apenas Minúsculas" for lowercase only
   - Leave both off for both cases
5. **Add combinations** (optional):
   - Toggle "Incluir Combinações" on
   - Enter letter combinations separated by commas
6. **Click "Gerar Folhas de Prática"** (Generate Practice Sheets)
7. **Print or Save as PDF** from your browser (Ctrl/Cmd+P)

## Page Format

Each page contains:
- **Default mode**: 3 lines of uppercase + 3 lines of lowercase (6 lines total)
- **Single case mode**: 6 lines of the selected case
- Each line shows: Example letter + guide lines for practice
  - Example: `A__________________________________________________`

## Technical Details

- Pure HTML/CSS/JavaScript - no build process needed
- Uses Google Fonts API for font loading
- Print-optimized CSS with A4 page sizing
- Font guide lines rendered using underscore character (`_`)
- Grey color preserved in print using `print-color-adjust: exact`

## Font Requirements

Works best with Google Fonts that have built-in guide lines for handwriting practice, such as:
- **Playwrite PT Guides** (recommended for Portuguese)
- **Playwrite PT**
- Other handwriting/cursive fonts

The underscore character (`_`) in these fonts displays as three horizontal guide lines, perfect for letter practice.

## Browser Compatibility

Tested and working in:
- Chrome/Edge
- Firefox
- Safari

## Language

The interface is in Portuguese (PT) but can easily be adapted to other languages by editing the HTML text labels.

## License

Feel free to use, modify, and share this project for educational purposes.

## Credits

Created for my daughter's handwriting practice. Hope it helps other parents and teachers too!
