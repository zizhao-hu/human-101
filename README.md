# Human 101

A tiny tutorial site for staying human when AI can do everything.

Each "skill" is a single copy-pasteable prompt plus an example multi-turn conversation showing how the prompt actually plays out. The goal isn't to teach you AI — it's to teach you the small human skills (asking, deciding, disagreeing, noticing what you actually feel) that the AI era quietly atrophies.

## View

Open `index.html` in any browser. No build step, no dependencies.

Live: https://zizhao-hu.github.io/human-101/ (after enabling GitHub Pages)

## Structure

- `index.html` — the whole site. Single self-contained file. Content lives in the `SKILLS` array near the top of the `<script>` block.

## Contributing a skill

Add an entry to the `SKILLS` array in `index.html`:

```js
{
  id: "short-unique-id",
  name: "Short skill title",
  why: "One short paragraph on why the skill matters.",
  prompt: "The copy-pasteable prompt the reader will use with their AI.",
  convo: [
    { role: "you", text: "..." },
    { role: "ai",  text: "..." }
  ],
  takeaway: "One sentence the reader should leave with."
}
```

Keep prompts concrete, short, and usable as-is. Example conversations should sound like real chats, not ad copy.

## License

MIT.
