# You Are the AI

A talk for teenagers (written for a scout group) on how chatbots and other AI systems work. Each scout plays one part of the AI: Guessers, Word Finders, Attention, Researchers and Agents. An animated slideshow sets up each part.

**Slides on GitHub Pages:** https://andy-thomason.github.io/scouts-ai-talk/

**Claude deck:** https://claude.ai/artifact/75Au5vHbDepAQ5t8UftLwY

## Presenting

Open the Pages link and press **F** for full screen. Use the arrow keys, space or a click to move on (slides with reveals step through them first), and press **N** to show the speaker notes. You can link straight to a slide with `#slide-7`. To run it offline, serve the folder locally, for example `python3 -m http.server`, and open http://localhost:8000.

## What's covered

1. **Guessing the next word**: a chatbot just guesses the next word. Story game starting from "Once upon a time".
2. **Word homes and attention**: every word has a home address, and similar words live close together. "What is the capital of France?" shows that every capital is the same step away from its country.
3. **Looking things up**: "Where can I buy a loaf of bread?" uses your location, a web search and opening times.
4. **Agents**: booking a train and sending emails, always asking before paying.
5. **Making pictures**: a diffusion model turns noise into a cat on a fence.
6. **Embodied AI**: humanoid robots (with a focus on the Chinese companies leading the next wave), Nvidia's duck robot Blue, and an "AI apocalypse" slide: *perhaps not this :)*

The game instructions for each part are in the speaker notes (the `<aside>` at the end of each slide). [NOTES.md](NOTES.md) has the original brief.

## Layout

- `index.html`: the standalone viewer. It loads `deck.json` and the slides, scales them to the window and runs the animations in sandboxed iframes.
- `deck.json`: slide order, sections and fonts (Fredoka and Nunito Sans from Google Fonts).
- `slides/<id>.html`: one slide each, a 1920×1080 `<section>` with inline styles. The animations are self-contained `<x-embed>` pages with plain JavaScript and no dependencies.
- `images/`: the photos. Slides refer to them by their uploaded asset URLs (`/_blob/<id>`):

| Image | Asset id |
|---|---|
| `images/agibot.jpg` | `7377d471f8348210ebbd439efe2a3c15` |
| `images/asimo.jpg` | `497b7986ab9b8f338c590ad9fe0a87d4` |
| `images/atlas.jpg` | `b504f257b0973c180438cb241ebd38dc` |
| `images/bdx.jpg` | `f109b20c465b81815ec316ad3a451690` |
| `images/g1.jpg` | `c750fe774be20da5dda5a3c6f3422184` |
| `images/galbot.jpg` | `7365cb6847d5357a4dc6f43e8ea60732` |
| `images/optimus.jpg` | `1fd4d3ae7a52531d45962803c859707f` |
| `images/wotw14.jpg` | `5bb08caccdb221944e38cd9523160f2a` |

## Image credits

All photos come from Wikimedia Commons and were cropped and resized for the slides.

- ASIMO at Honda Collection Hall, by Syced, CC0
- Boston Dynamics Atlas, by Damian B Oh, CC BY-SA 4.0
- Tesla Optimus, by Benjamin Ceci, public domain
- Unitree G1, by Sayanesy, CC0
- AgiBot X2 at MWC 2026, by JJxFile, CC BY 4.0
- Galbot drinks kiosk in Shenzhen, by SABAIEE HuangChuis MMADEEG, CC0
- BDX droids at Disneyland, by Contributor19, CC BY 4.0
- *The War of the Worlds* illustration (1906), by Henrique Alvim Corrêa, public domain

The CC BY and CC BY-SA images need the credit kept with them when reused. `images/atlas.jpg` is a cropped version of a CC BY-SA 4.0 photo, so it stays under CC BY-SA 4.0.
