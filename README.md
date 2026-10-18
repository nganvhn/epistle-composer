# Epistle Composer

A mobile UI design and interactive prototype for **Epistle**, an app that writes a letter for you. Pick who it's for, pick a tone, jot down what you want to say, and Epistle drafts the letter.

## The flow

1. **Setup.** Choose a recipient (Spouse, Parent, Colleague, Friend, and more), choose a tone (Gentle, Witty, Formal, Apologetic, and more), then write a few rough lines in the message box.
2. **Writing.** A short loading screen shows ink strokes being drawn on paper, with a Cancel button to go back.
3. **Result.** The drafted letter appears in a serif "paper" card. From there you can:
   - switch tone from a dropdown that floats over the letter, so nothing shifts,
   - try another phrasing,
   - edit the letter inline,
   - copy the text (a toast confirms it),
   - share it by email, message, or PDF from a bottom sheet.

Your recipient, tone, and message are kept when you go back to edit details.

## Design notes

- **Palette:** warm cream background, near-black ink, white surfaces, soft beige borders.
- **Type:** Source Serif 4 for the wordmark, headline, and letters; Work Sans for interface text.
- **Shape:** fully rounded pills for chips and buttons, large radii on cards and sheets.
- **Icons:** Feather icon set, 2px stroke with round caps and joins.
- **Layout:** 390 x 844 phone artboard, 44px minimum tap targets.

## Files

| File | What it is |
| --- | --- |
| `project/Main.dc.html` | The whole prototype: all three screens, their states, and the sample letters. |
| `project/canvas.json` | Canvas layout (artboard size and position, title). |

The `.dc.html` format is made for the Claude Design canvas. Its `support.js` runtime is provided by the canvas, so opening `Main.dc.html` directly in a browser won't render it. Treat these files as design source to import back into a canvas.

## Prototype limits

This is a design prototype, not a working product. There is no AI behind it. The letters are written samples for four tones (Gentle, Witty, Formal, Apologetic), each with two phrasings. The other tones reuse the Witty sample. The share options don't send anything.
