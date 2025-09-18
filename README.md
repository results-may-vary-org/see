# SEE - Strategic Excellence Evaluation

A retro Windows 98-styled dashboard for tracking open source project tasks and GitHub issues, combining nostalgic aesthetics with modern project management functionality.

## Features

- 🎨 **Authentic Windows 98 styling** powered by 98.css
- 📝 **Dynamic task loading** from JSON with smooth loading states
- 🐛 **GitHub issues integration** for community feedback visibility
- ⏰ **Real-time clock** and project status indicators
- 📊 **Priority metrics** for efficient task management
- 🔧 **Professional interface** suitable for team collaboration

## Quick Start

1. Clone this repository
2. Open `index.html` in your browser (serve via HTTP for JSON loading)
3. View your organized project dashboard

## Customization

### Update Your Tasks

Edit `todos.json` with your project tasks:

```json
[
  {
    "name": "Your project task",
    "description": "Clear description of the work to be done",
    "project": "project-name",
    "link": "https://github.com/user/repo",
    "priority": "high",
    "created": "2024-12-18"
  }
]
```

### Add Your GitHub Repositories

Update the `repos` array in `index.html` around line 255:

```javascript
const repos = [
    'yourUsername/your-repo',
    'yourUsername/another-repo'
];
```

### Interface Customization

Modify colors, fonts, and layout in the CSS section to match your team's preferences.

## Development Setup

Since this loads JSON files locally, you'll need to serve it via HTTP:

```bash
# Python 3
python -m http.server 8000

# Node.js (with http-server)
npx http-server

# PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

## Use Cases

- **Project Management**: Track development tasks across multiple repositories
- **Team Collaboration**: Share project status with team members and stakeholders
- **Community Engagement**: Display open issues for community contributors
- **Status Dashboard**: Monitor project health and development progress

## Technical Details

- Pure HTML, CSS, and JavaScript (no build process required)
- GitHub API integration for real-time issue fetching
- JSON-based configuration for easy maintenance
- Responsive design that works across devices
- No external dependencies except 98.css CDN

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for improvements.

## License

MIT - Open source software for collaborative development.

---

*A nostalgic approach to modern project management, bringing the charm of classic interfaces to contemporary development workflows.*