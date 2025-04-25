# Whimsical April 2022 Quiz

An interactive, browser-based quiz celebrating quirky news and traditions from April 2022. Built with plain HTML, Tailwind CSS and vanilla JavaScript (plus canvas-confetti for the final celebration!).

## Features

- Multiple-choice questions with animated fade-ins
- Placeholder (or real) images alongside each question detail
- Confetti effect on completion
- Custom fonts (Cosmica Bold for headings, Plus Jakarta Sans for body)
- Easy styling and layout via Tailwind utilities

## Running Locally

1. Clone or download this repo.
2. Ensure the font files (`Cosmica-Bold.woff2` and `PlusJakartaSans-VariableFont_wght.woff2`) and any question images are in the project root.
3. Open `quiz.html` in any modern browser (no build step required).

## Adding or Editing Questions

All questions live in the `questions` array at the top of `quiz.html`. Each item is an object with these fields:

```js
{
  question: "Your question text",
  options: ["Choice A", "Choice B", "Choice C", "Choice D"],
  answer: 0,          // zero-based index of correct option
  detail: "Explanation or fun fact with **markdown** for bold text.",
  photo: "https://link-to-your-image.jpg"
}
```

### Using ChatGPT to Generate New Content

You can ask ChatGPT for fresh quiz entries. For example:

> "Generate 3 April 2023 quiz questions in JSON format, each with question, four options, an answer index, a detail string, and a placeholder image URL."

Then paste the returned array items directly into the `questions` array in `quiz.html`.

## Customization

- **Styling**: Modify Tailwind classes on containers or elements.
- **Animations**: Adjust or add more CSS keyframes in the `<style>` block.
- **Fonts**: Swap out or add new `@font-face` rules in the `<head>` section.

---

*Have fun editing and expanding this quiz! Feel free to open issues or pull requests on GitHub.*
