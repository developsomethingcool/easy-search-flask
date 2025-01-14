# Web Crawler Search Application

A Flask-based web application that crawls websites, indexes their content using Whoosh, and provides a beautiful search interface.

## Description

This application combines web crawling capabilities with a modern search interface. It crawls specified websites, indexes the content using Whoosh for full-text search, and presents results through an animated UI.

## Features

- 🕷️ Web crawling with rate limiting
- 🔍 Full-text search using Whoosh
- ✨ Modern, animated search interface
- 📱 Responsive design
- 🎨 Dynamic UI effects

## Installation

```bash
# Clone the repository
git clone https://github.com/developsomethingcool/easy-search-flask
cd easy-search-flask

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install required packages
pip install flask requests beautifulsoup4 whoosh
```

## Usage

1. Start the Flask application:
```bash
python flask_app.py
```

2. Open `http://localhost:5000` in your browser
3. Enter search terms to find content from the crawled website

## Project Structure

```
├── crawler.py           # Web crawler and indexing logic
├── flask_app.py         # Flask application
├── static/
│   ├── styles.css      # CSS styles
│   └── scripts.js      # UI effects
├── templates/
│   ├── search_form.html    # Search interface
│   └── search_results.html # Results page
└── indexdir/           # Search index directory
```

## Configuration

Edit `flask_app.py` to configure the base URL:
```python
base_url = "https://vm009.rz.uos.de/crawl/index.html"
index_dir = "indexdir"
```

## Requirements

- Python 3.6+
- Flask
- BeautifulSoup4
- Whoosh
- Requests

## Browser Support

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.
