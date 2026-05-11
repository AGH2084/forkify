# forkify Project

Recipe application to search, view, bookmark, and upload recipes. Built with modern JavaScript, SCSS, and Parcel bundler.

## Features
- Search over 1,000,000 recipes
- View detailed recipe instructions and ingredients
- Bookmark favorite recipes
- Upload your own custom recipes
- Responsive and modern UI

## Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v14 or higher recommended)

### Installation
1. Clone the repository:
	```bash
	git clone https://github.com/your-username/forkify.git
	```
2. Navigate to the project folder:
	```bash
	cd forkify
	```
3. Install dependencies:
	```bash
	npm install
	```

### Running the App
Start the development server:
```bash
npm run start
```
The app will open at `http://localhost:1234` by default.

## Folder Structure

```
forkify/
├── index.html
├── package.json
├── src/
│   ├── img/           # Images and icons
│   ├── js/            # JavaScript source files
│   │   ├── config.js
│   │   ├── controller.js
│   │   ├── helpers.js
│   │   ├── model.js
│   │   └── views/     # View components
│   └── sass/          # SCSS styles
└── README.md
```

## Technologies Used
- JavaScript (ES6+)
- SCSS (Sass)
- Parcel (bundler)
- [core-js](https://github.com/zloirock/core-js) for polyfills
- [fractional](https://www.npmjs.com/package/fractional) for ingredient fractions

## Author
Armin Ghapani

## License
ISC
