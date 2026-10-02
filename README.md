# Word Counter v1

A React word & character counter component built with [shadcn/ui](https://ui.shadcn.com/) primitives — paste-ready for any Next.js / React + Tailwind project. It renders a textarea with live text statistics: words, characters (with or without spaces), sentences, paragraphs, estimated reading time, and a character-limit progress bar with a long-text warning.

## Features

- **Live stats** — word, character, sentence, and paragraph counts update on every keystroke
- **Space toggle** — include or exclude whitespace from the character count
- **Reading-time estimate** — selectable reading speed (100 / 200 / 300 wpm)
- **Progress bar** — visual length indicator against a 10,000-character guideline (green → yellow → red)
- **Long-text warning** — alert card when text exceeds 8,000 characters
- **Clear button** — one click to reset the textarea

## Tech Stack

- React 18 (hooks: `useState`, `useEffect`)
- shadcn/ui components — `Button`, `Card`, `Label`, `Textarea`, `Select`
- Tailwind CSS utility classes
- ES modules

## Quick Start

The component file (`word-counter v1`) exports a default `WordCounter` component. Drop it into any React + Tailwind + shadcn/ui project:

```tsx
import WordCounter from './WordCounter'

export default function Page() {
  return <WordCounter />
}
```

Requirements in the host project:

- shadcn/ui components installed: `button`, `card`, `label`, `textarea`, `select`
- The `@/` path alias pointing at your project root (adjust the imports if yours differs)
- Tailwind CSS with the shadcn theme variables (`bg-background`, `text-foreground`, `text-muted-foreground`, …)

Note: two imports in the file are inconsistent (`"/components/ui/..."` vs `"@/components/ui/..."`) — normalize them to your project's alias when copying.

## Project Structure

```
word-counter-v1/
├── word-counter v1   # the WordCounter React component
├── LICENSE           # CC license
└── README.md         # this file
```

## License

See `LICENSE` for details.

---

Built by Girish Lade — https://ladestack.in
