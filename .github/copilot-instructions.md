# Keeper - Copilot Instructions

## Known bug: Input element destruction on re-render

When rendering transaction log inputs, **never rebuild input elements on every keystroke**. The previous bug was that `renderLog` rebuilt all inputs on every `input` event, destroying the DOM elements and losing cursor/focus.

**Correct pattern:**
- **Input changes** (credit, debit, amount fields) → only re-render the summary (text-only elements, no inputs)
- **Add/delete rows** → re-render the log (since the DOM structure actually changes)

The input elements should persist across keystrokes. Only the balance summary (which is text-only) should be rebuilt on every transaction change.
