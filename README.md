# Gabinete

Gabinete is a mockup of a small app to listen to podcasts about curiosities: science, history, nature, language, the human body and space.
I built it only with HTML and CSS for the DIW course (DAW, CEI).

## Live demo

https://ruizdelavegaalba-png.github.io/Gabinete/

## Screenshots

### Home

![Home page](screenshots/index.png)

### Podcast

![Podcast page](screenshots/podcast.png)

### Episode

![Episode page](screenshots/episode.png)

### Mobile

![Mobile view](screenshots/mobile.png)

## Pages

- **index.html**: the featured episode, a search field, 12 podcast cards and the popular categories.
- **podcast.html**: the information of each podcast and a table with its 10 episodes.
- **episode.html**: each episode with its description, an audio player and a transcript.
- **categories.html**: 6 categories with their podcasts.
- **library.html**: 3 episodes to continue listening and 4 favourite podcasts.
- **authors.html**: a card for each of the 12 authors.
- **about.html**: our mission, our values and a contact form.

## Project structure

```
Gabinete/
├── index.html
├── podcast.html
├── episode.html
├── categories.html
├── library.html
├── authors.html
├── about.html
├── styles.css
├── screenshots/
└── README.md
```

## How to view it

- Open `index.html` in Google Chrome.
- Or open the folder in VS Code and use the Live Server extension.

You need an internet connection, because the images, the audio and the fonts are online.

## How it works without JavaScript

All 12 podcasts are in `podcast.html` and all 120 episodes are in `episode.html`. Each one is a block with its own id, and the links point to that id, for example `podcast.html#mitosAlMicroscopio`. With CSS I hide all the blocks and I only show the one in the link with `:target`. If there is no id in the link, `:has` shows a default block.

```css
.podcast {
    display: none;
}

.podcast:target {
    display: flex;
}
```

## What I learned

- How to build layouts with Flexbox and CSS Grid.
- How to show different content without JavaScript using `:target` and `:has`.
- How to work with Git branches: one branch for each part, merged into `dev`.
- Basic accessibility: one `h1` per page, alt texts, labels, visible focus and transcripts.
- How to make a responsive website with media queries.

## Things to improve

- Make the search field and the contact form work with JavaScript.
- Use a different audio file for each episode.
- Load the podcasts and episodes from a JSON file.
- Save the favourites and the listening progress for each user.
- Add a light and dark mode switch.

## Credits

- Voices generated with ElevenLabs.
- Images and logo created for this project.
- Images and audio hosted on Cloudinary.
- Fonts from Google Fonts (Barlow and Barlow Condensed).

## Author

Alba Ruiz de la Vega · DAW · CEI · 2026
