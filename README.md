# Gabinete

Gabinete is a mockup of a small app to listen to podcasts about curiosities: science, history, nature, language, the human body and space.
I built it only with HTML and CSS for the DIW course (DAW, CEI).

## Live demo

[https://ruizdelavegaalba-png.github.io/Gabinete/](https://ruizdelavegaalba-png.github.io/Gabinete/)

## Screenshots

### Home

<img width="1895" height="905" alt="image" src="https://github.com/user-attachments/assets/f96fb756-19d3-4c2d-819c-19cefa0f6919" />


### Podcast

<img width="1886" height="897" alt="image" src="https://github.com/user-attachments/assets/15bcb49c-c84f-498f-88db-aab122a218bf" />


### Episode

<img width="1876" height="898" alt="image" src="https://github.com/user-attachments/assets/9a14a753-859d-454e-a8b5-0f061e1a71ae" />

### Categories
<img width="1877" height="902" alt="image" src="https://github.com/user-attachments/assets/e43b23e1-a99e-48d9-bb95-b4030b56a00d" />


### Library
<img width="1886" height="898" alt="image" src="https://github.com/user-attachments/assets/3763c7e2-e169-4751-97a1-c2ca8144b8a3" />


### Authors
<img width="1890" height="906" alt="image" src="https://github.com/user-attachments/assets/346fea5d-21fe-459b-97b2-028a5effd1cb" />

### Us
<img width="1891" height="895" alt="image" src="https://github.com/user-attachments/assets/9d2f1242-78a2-4500-953f-e1a2f7054e2d" />


### Mobile

<img width="1107" height="2048" alt="WhatsApp Image 2026-11-16 at 12 30 51" src="https://github.com/user-attachments/assets/70799459-d572-45b7-b72a-fd1f6c608c91" />


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
- Load the podcasts and episodes from a JSON file.
- Save the favourites and the listening progress for each user.
- Add a light and dark mode switch.

## Credits

- Each episode has its own audio, generated with ElevenLabs. The flamingos episode is a dialogue with two voices.
- Images and logo created for this project.
- Images and audio hosted on Cloudinary.
- Fonts from Google Fonts (Barlow and Barlow Condensed).

## Author

Alba Ruiz de la Vega · DAW · CEI · 2026
