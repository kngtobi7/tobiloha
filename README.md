# Verdant — Wellness Studio 🌿

A responsive, green-and-white wellness website for meal inspiration, BMI estimates, food nutrient estimates, movement ideas and nearby food discovery.

## Features

- **Meal planner:** creates flexible breakfast, lunch, dinner and snack ideas based on age group, food preference and foods to avoid.
- **BMI calculator:** calculates BMI from metric height and weight. Adult reference ranges are shown only for adults; under-20 results are not classified because they require age- and sex-specific growth-chart percentiles.
- **Nutrition tracker:** add foods and servings to estimate calories, protein, carbohydrates, fat and fibre.
- **Movement suggestions:** beginner, moderate and active exercise ideas.
- **Nearby food spots:** uses browser geolocation and OpenStreetMap's public Overpass API to find mapped restaurants, cafés and fast-food locations around you.
- **Responsive layout:** designed for desktop, tablet and mobile.

## Run locally

No build step or package installation is required.

1. Download or clone this repository.
2. Open `index.html` in a browser.

For the nearby places feature, browser geolocation generally requires a secure context (`https://` or `localhost`). If opening the file directly does not allow location access, run a local server:

```bash
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`, `styles.css`, `app.js` and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Wait for GitHub Pages to publish your site.

## Data and privacy notes

- BMI, meal ideas and nutrient calculations run locally in your browser. This demo does not create an account or send these entries to a server.
- Location is requested only when the visitor presses **Find near me**. Coordinates are sent to the public OpenStreetMap Overpass endpoint to retrieve nearby mapped food places.
- Google Fonts are loaded from Google Fonts when internet access is available.
- Food nutrient figures are approximate generic averages, not laboratory values. Brands, recipes, portions and preparation methods change nutrient content.
- Restaurant data is community-maintained OpenStreetMap data and may be incomplete or outdated. Verify opening hours, menus, contact details and dietary suitability directly with the venue.

## Important health and safety disclaimer

Verdant is an educational wellness demo, not a medical device and not a substitute for a registered dietitian, doctor or qualified exercise professional. It does not diagnose, treat or prevent disease, and it does not prescribe calorie targets.

BMI is a screening measure, not a diagnosis. For children and teens, BMI interpretation requires age- and sex-specific growth-chart percentiles; this app intentionally does not label their BMI. Meal suggestions for children, teens, older adults, pregnancy, allergies or medical conditions should be reviewed by a qualified professional or caregiver as appropriate. Exercise should be adapted to the person's ability and health status.

## Project structure

```text
verdant-wellness/
├── index.html
├── styles.css
├── app.js
└── README.md
```

## Built with

- HTML5
- CSS3
- Vanilla JavaScript
- OpenStreetMap / Overpass API for nearby places

## License

You may use, adapt and extend this starter project. Add a license file if you want to specify formal reuse terms for your public repository.
