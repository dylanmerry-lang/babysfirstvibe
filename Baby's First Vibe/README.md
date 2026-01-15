# IT Tips & Tricks Tracker

A web application for tracking common IT support issues and their ChatGPT solutions. Perfect for IT support teams to maintain a knowledge base of frequently encountered problems and their resolutions.

## Features

- 📋 **Tip Management**: Store and organize IT tips with problem descriptions and solutions
- 🔍 **Search & Filter**: Quickly find tips by title, problem description, or category
- 📱 **Responsive Design**: Works on desktop, tablet, and mobile devices
- 🎨 **Clean UI**: Modern, intuitive interface for easy navigation
- 💾 **Local Storage**: JSON-based storage for simplicity and portability
- ⚡ **Fast & Lightweight**: No heavy frameworks, pure JavaScript

## Technology Stack

- **Backend**: Node.js + Express.js
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Storage**: JSON file (easily upgradeable to database)
- **Styling**: Custom CSS with responsive design

## Quick Start

### Prerequisites
- Node.js (v14 or higher)
- npm (comes with Node.js)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/dylanmerry-lang/babysfirstvibe.git
   cd babysfirstvibe
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

4. **Open your browser**
   Navigate to `http://localhost:3000`

## Usage

### Viewing Tips
- Browse all IT tips on the main page
- Click on any tip card to view full details
- Use the search bar to find specific tips
- Filter by category using the dropdown

### Adding New Tips
- Click "Add New Tip" button
- Fill in the form with:
  - **Title**: Brief description of the issue
  - **Category**: Problem category (Windows, Hardware, etc.)
  - **Problem**: Detailed problem description
  - **ChatGPT Answer**: The solution provided by ChatGPT

### Managing Tips
- All tips are stored locally in JSON format
- Data persists between server restarts
- Easy to backup and migrate

## Project Structure

```
babysfirstvibe/
├── server/
│   └── app.js                 # Express server and API routes
├── public/
│   ├── index.html            # Main HTML page
│   ├── css/
│   │   └── styles.css        # Application styles
│   └── js/
│       └── app.js            # Frontend JavaScript
├── data/
│   └── tips.json             # Tips storage
├── package.json              # Dependencies and scripts
├── README.md                 # This file
└── .gitignore               # Git ignore rules
```

## API Endpoints

- `GET /api/tips` - Retrieve all tips
- `GET /api/tips/:id` - Retrieve single tip
- `POST /api/tips` - Create new tip
- `PUT /api/tips/:id` - Update existing tip
- `DELETE /api/tips/:id` - Delete tip

## Sample Data

The application comes with sample IT tips including:
- Windows Update issues
- Printer connectivity problems
- Outlook email sending issues

## Development

### Available Scripts

- `npm start` - Start the production server
- `npm run dev` - Start development server (same as start)

### Customization

- **Categories**: Edit the category options in `public/index.html` and `public/js/app.js`
- **Styling**: Modify `public/css/styles.css` for custom appearance
- **Storage**: Replace JSON storage with database in `server/app.js`

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

MIT License - feel free to use for personal or commercial projects.

## Support

For questions or issues:
- Check the browser console for errors
- Verify Node.js and npm are properly installed
- Ensure port 3000 is not in use by other applications

## Future Enhancements

- [ ] User authentication and authorization
- [ ] Database integration (MongoDB, PostgreSQL)
- [ ] Tip voting and rating system
- [ ] Export functionality (PDF, CSV)
- [ ] Advanced search with filters
- [ ] Tip categories management
- [ ] Backup and restore features