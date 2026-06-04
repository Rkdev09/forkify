# Forkify

A recipe search web app built with vanilla JavaScript. Search over 1,000,000 recipes, view details, adjust servings, bookmark favorites, and upload your own recipes.

## Features

- Search recipes by keyword
- View recipe details with ingredients and directions
- Update servings (quantities scale automatically)
- Bookmark recipes (saved in localStorage)
- Pagination for search results
- Upload custom recipes (requires API key)

## Tech Stack

- HTML, SCSS, JavaScript (ES modules)
- [Parcel](https://parceljs.org/) — bundler
- [Forkify API](https://forkify-api.jonas.io/) — recipe data
- MVC architecture (Model, Views, Controller)

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or later recommended)

### Installation

```bash
git clone https://github.com/Rkdev09/forkify.git
cd forkify
npm install
```

### Development

```bash
npm start
```

Open [http://localhost:1234](http://localhost:1234) in your browser.

### Production Build

```bash
npm run build
```

Output is written to the `dist/` folder.

## API Key (optional)

To upload your own recipes, get an API key from [forkify-api.jonas.io](https://forkify-api.jonas.io/) and set it in `src/js/config.js`:

```js
export const KEY = 'your-api-key-here';
```

Search and viewing recipes work without an API key.

## Project Structure

```
starter/
├── index.html
├── src/
│   ├── js/
│   │   ├── controller.js   # App logic & event handlers
│   │   ├── model.js        # State & API calls
│   │   ├── config.js       # API URL, timeouts, etc.
│   │   ├── helpers.js      # AJAX helper
│   │   └── views/          # UI components
│   ├── sass/               # Styles
│   └── img/                # Icons & assets
└── package.json
```

## Author

Ritika Mishra

## License

ISC
