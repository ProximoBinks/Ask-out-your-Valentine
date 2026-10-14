# Valentine's Day Interactive Website (CodeKage)

A cute, interactive web page to ask someone to be your Valentine. Features playful button mechanics, heartwarming GIFs, and heart-shaped confetti.

## How It Works

1. The page presents the question **"Will you be my Valentine?"** alongside a cute GIF.
2. Clicking **No** swaps the GIF, changes the button text to increasingly desperate pleas, and grows the **Yes** button bigger and bigger.
3. Clicking **Yes** celebrates with a special GIF, a victory message, and a burst of heart-shaped confetti.

## Features

- **Growing "Yes" button** -- gets larger with every "No" click, making it impossible to ignore.
- **Desperate messages** -- the "No" button cycles through pleading texts like *"Pookie please"* and *"I'm gonna cry..."*.
- **Animated GIFs** -- seven different GIFs that react to the user's choices.
- **Heart confetti** -- pink heart-shaped confetti explosion on "Yes" using [canvas-confetti](https://www.npmjs.com/package/canvas-confetti).
- **Responsive design** -- looks great on desktop and mobile, powered by [Tailwind CSS](https://tailwindcss.com).

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/CodeKageHQ/Ask-out-your-Valentine.git
   ```
2. Open `index.html` in your browser.

That's it -- no build step, no dependencies to install. Tailwind CSS and canvas-confetti are loaded via CDN.

## Project Structure

```
Ask-out-your-Valentine/
├── images/
│   ├── image1.gif    # Default greeting
│   ├── image2.gif    # After 1st "No"
│   ├── image3.gif    # After 2nd "No"
│   ├── image4.gif    # After 3rd "No"
│   ├── image5.gif    # After 4th "No"
│   ├── image6.gif    # After 5th "No"
│   └── image7.gif    # "Yes" celebration
├── index.html        # The entire app (HTML + CSS + JS)
├── LICENSE
└── README.md
```

## Customization

Want to make it your own? Here are some easy tweaks inside `index.html`:

| What | Where | How |
|------|-------|-----|
| GIF images | `images/` folder | Replace the GIFs with your own (keep the same filenames) |
| "No" button messages | `NO_BUTTON_MESSAGES` array | Edit the strings to say whatever you like |
| Button growth speed | `GROWTH_PER_CLICK` / `FONT_GROWTH_PER_CLICK` constants | Lower the numbers for subtler growth |
| Confetti colors | `colors` array in the `yesButton` click handler | Swap in any hex color codes |
| Background gradient | `.gradient-background` in `<style>` | Change the hex colors |

## Technologies

- **HTML5** -- semantic markup with `<main>` and `<section>`
- **Tailwind CSS** -- utility-first styling via CDN
- **JavaScript** -- vanilla JS, no frameworks
- **canvas-confetti** -- lightweight confetti animation library

## Contributing

Contributions are welcome! Whether it's new GIF suggestions, design tweaks, or code improvements -- fork the repo and open a pull request.

## Star History

<a href="https://www.star-history.com/?type=date&amp;repos=ProximoBinks%2FAsk-out-your-Valentine">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ProximoBinks/Ask-out-your-Valentine&amp;type=date&amp;theme=dark&amp;legend=top-left" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ProximoBinks/Ask-out-your-Valentine&amp;type=date&amp;legend=top-left" />
    <img alt="Star History Chart for Ask-out-your-Valentine" src="https://api.star-history.com/chart?repos=ProximoBinks/Ask-out-your-Valentine&amp;type=date&amp;legend=top-left" />
  </picture>
</a>

## License

Open source under the [MIT License](LICENSE).

Happy Valentine's Day! ❤️
