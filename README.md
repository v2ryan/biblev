# Parallel Bible Reader

A modern web application for reading and comparing Bible translations side by side.

## Features

- **Dual-Pane View**: Compare two Bible versions simultaneously
- **Left Pane**: Browse 100+ Bible translations from local JSON files
- **Right Pane**: Access Chinese Bible versions via hb.fhl.net API
- **Easy Navigation**:
  - Navigate by book and chapter
  - Use Previous/Next buttons
  - Keyboard shortcuts (← → arrow keys)
- **Clean Interface**: Modern, responsive design that works on desktop and mobile
- **Multiple Versions**: Support for KJV, ASV, Chinese versions (和合本, 新標點和合本), and many more

## Usage

### Local Development

1. Clone the repository
2. Start a local web server:
   ```bash
   python -m http.server 8000
   ```
3. Open http://localhost:8000 in your browser

### Deployment

The app is deployed on Vercel and can be accessed at your deployment URL.

## Project Structure

```
biblev/
├── index.html          # Main application file
├── json/              # Bible translation JSON files (100+ versions)
│   ├── KJV.json
│   ├── ASV.json
│   ├── ChiUn.json
│   └── ...
├── vercel.json        # Vercel deployment configuration
└── README.md          # This file
```

## API Integration

The right pane uses the Bible API from [https://hb.fhl.net/api/](https://hb.fhl.net/api/) to fetch Chinese Bible translations in real-time.

## Technologies

- HTML5
- CSS3 (Flexbox, Grid)
- Vanilla JavaScript (ES6+)
- Fetch API for data loading

## License

This project is open source and available for educational and personal use.

## Credits

- JSON Bible files from [scrollmapper/bible_databases](https://github.com/scrollmapper/bible_databases)
- Chinese Bible API from [hb.fhl.net](https://hb.fhl.net/)
