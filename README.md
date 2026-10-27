# About Me & My Town

A small React app with two views, **About Me** and **My Town**. My Town shows
the current weather from the free [Open-Meteo](https://open-meteo.com/) API
(no key needed), an image based on the temperature, and a °C/°F toggle.

**Live site:** https://fascinating-manatee-c1bda3.netlify.app/

## How it works
- `src/App.jsx` holds everything: the two views, navigation (a `page` state), the `fetch` call, the image choice, and the unit toggle.
- Image rule (Celsius): ≤ 10 → `cold.png`, 11–19 → `mild.png`, ≥ 20 → `sunny.png`.
- `src/style.css` has the styling.

## Run
```bash
npm install
npm run dev      # development
npm run build    # outputs /dist
```
Put `cold.png`, `mild.png`, `sunny.png` in `public/`, and edit the name, bio, town, and coordinates in `src/App.jsx`.

## Deploy
Run `npm run build` and drag the `dist` folder to https://app.netlify.com/drop (or import the GitHub repo on Vercel).

## AI disclosure
Before coding, I made a low-fidelity sketch of the website's layout and user journey. 
I then used Claude (Anthropic) to generate the code for the app and this README, working from the assignment rubric.
I ran the app locally, tested both pages, the weather image and the °F button, and deployed it to Netlify myself.
I edited the content and coordinates to match my town.