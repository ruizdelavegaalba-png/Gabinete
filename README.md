# Gabinete

Gabinete is a mockup of a small app to listen to podcasts about curiosities: science, history, nature, language, the human body and space.
I built it only with HTML and CSS for the DIW course (DAW, CEI).

## Live demo

[https://ruizdelavegaalba-png.github.io/Gabinete/](https://ruizdelavegaalba-png.github.io/Gabinete/)

## Screenshots

### Home

<img width="1881" height="910" alt="image" src="https://github.com/user-attachments/assets/f334b542-fe7f-4ed8-9812-b3c346615b81" />



### Podcast

<img width="1877" height="907" alt="image" src="https://github.com/user-attachments/assets/85cac2fc-d9c7-4d43-bfcd-f2a6d6bcaa06" />



### Episode

<img width="1877" height="865" alt="image" src="https://github.com/user-attachments/assets/e718fbf3-50d1-4eab-91e0-084338f5c619" />


### Categories
<img width="1865" height="891" alt="image" src="https://github.com/user-attachments/assets/63bc0101-0bd5-4e11-b122-e67ba8050b09" />



### Library
<img width="1872" height="880" alt="image" src="https://github.com/user-attachments/assets/eaf8cbed-d3a0-440b-a0fe-0a2d4ae69704" />



### Authors
<img width="1868" height="896" alt="image" src="https://github.com/user-attachments/assets/fc7012a4-6c34-4138-aa33-c33598bbc261" />


### Us
<img width="1872" height="892" alt="image" src="https://github.com/user-attachments/assets/a9aa1955-3716-4c91-b525-75dd7803ef5f" />



### Mobile

<img width="857" height="1600" alt="Image 2026-11-19 at 10 18 25" src="https://github.com/user-attachments/assets/add57f2c-8c32-4d68-a05d-40d2e0375cbd" />



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

All 12 podcasts are in `podcast.html` and all 120 episodes are in `episode.html`. Each one is a block with its own id, and the links point to that id, for example `podcast.html#mythsUnderTheMicroscope`. With CSS I hide all the blocks and I only show the one in the link with `:target`. If there is no id in the link, `:has` shows a default block.

```css
.podcast,
.podcastDefault {
    display: none;
}

.podcast:target,
.podcastList:not(:has(:target)) .podcastDefault {
    display: flex;
}
```

## Code names

All the names in the code (classes, ids and CSS variables) are in English and in camelCase, for example `cardTitle`, `backButton` or `--colorCyan`. The texts that the user sees are in Spanish (`lang="es"`).

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

---
## HTML validation

I checked all the pages with the [W3C Markup Validation Service](https://validator.w3.org/). All of them pass with no errors.

<img width="911" height="432" alt="image" src="https://github.com/user-attachments/assets/70027f91-1ac4-4722-b058-874dd2a3fe01" />

## Author

Alba Ruiz de la Vega 
