# Setup Instructions

This guide will help you set up the Secure Medical Data Sharing System on your local machine.

## Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v14.0.0 or higher)
  - Download from [nodejs.org](https://nodejs.org/)
  - Verify installation: `node --version`
  
- **npm** (v6.0.0 or higher) or **yarn** (v1.22.0 or higher)
  - npm comes with Node.js
  - Verify installation: `npm --version`
  
- **Git**
  - Download from [git-scm.com](https://git-scm.com/)
  - Verify installation: `git --version`

## Installation Steps

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/secure-medical-data-sharing.git
cd secure-medical-data-sharing
```

### 2. Install Dependencies

Using npm:
```bash
npm install
```

Or using yarn:
```bash
yarn install
```

This will install all required dependencies including:
- React
- React DOM
- Lucide React (for icons)
- Tailwind CSS (for styling)

### 3. Install Tailwind CSS

If not already configured, set up Tailwind CSS:

```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

### 4. Start the Development Server

Using npm:
```bash
npm start
```

Or using yarn:
```bash
yarn start
```

The application will automatically open in your default browser at:
```
http://localhost:3000
```

## Project Structure

After installation, your project structure should look like this:

```
secure-medical-data-sharing/
├── node_modules/          # Dependencies (auto-generated)
├── public/
│   ├── index.html        # HTML template
│   ├── favicon.ico       # Site icon
│   └── manifest.json     # PWA manifest
├── src/
│   ├── components/
│   │   └── SecureMedicalDataSharing.jsx  # Main component
│   ├── App.js            # Root component
│   ├── App.css           # App styles
│   ├── index.js          # Entry point
│   └── index.css         # Global styles
├── .gitignore            # Git ignore rules
├── package.json          # Project dependencies
├── tailwind.config.js    # Tailwind configuration
├── README.md             # Project documentation
├── LICENSE               # MIT License
├── CONTRIBUTING.md       # Contribution guidelines
└── SETUP.md              # This file
```

## Configuration

### Tailwind CSS Configuration

The `tailwind.config.js` file is already configured. If you need to customize:

```javascript
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {
      // Add your customizations here
    },
  },
  plugins: [],
}
```

### Environment Variables (Optional)

Create a `.env` file in the root directory if you need environment-specific configuration:

```env
REACT_APP_NAME=Secure Medical Data Sharing
REACT_APP_VERSION=1.0.0
```

## Building for Production

To create a production build:

Using npm:
```bash
npm run build
```

Or using yarn:
```bash
yarn build
```

This creates an optimized build in the `build/` directory ready for deployment.

## Deployment Options

### Deploy to GitHub Pages

1. Install gh-pages:
```bash
npm install --save-dev gh-pages
```

2. Add to `package.json`:
```json
"homepage": "https://yourusername.github.io/secure-medical-data-sharing",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
```

3. Deploy:
```bash
npm run deploy
```

### Deploy to Netlify

1. Build the project:
```bash
npm run build
```

2. Drag and drop the `build` folder to [Netlify](https://app.netlify.com/)

Or use Netlify CLI:
```bash
npm install -g netlify-cli
netlify deploy
```

### Deploy to Vercel

1. Install Vercel CLI:
```bash
npm install -g vercel
```

2. Deploy:
```bash
vercel
```

## Troubleshooting

### Common Issues

#### Port 3000 Already in Use

If port 3000 is already in use, you can:

1. Kill the process using port 3000
2. Or specify a different port:
```bash
PORT=3001 npm start
```

#### Module Not Found Errors

If you see module not found errors:

1. Delete `node_modules` and `package-lock.json`:
```bash
rm -rf node_modules package-lock.json
```

2. Reinstall dependencies:
```bash
npm install
```

#### Tailwind Styles Not Loading

Ensure `index.css` contains:
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

And it's imported in `index.js`:
```javascript
import './index.css';
```

#### React Version Conflicts

Ensure you're using compatible versions:
```bash
npm install react@latest react-dom@latest
```

## Running Tests

To run tests (if configured):
```bash
npm test
```

## Additional Resources

- [React Documentation](https://react.dev/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Create React App Documentation](https://create-react-app.dev/)
- [Lucide React Icons](https://lucide.dev/guide/packages/lucide-react)

## Getting Help

If you encounter any issues:

1. Check the [GitHub Issues](https://github.com/yourusername/secure-medical-data-sharing/issues)
2. Read the [Contributing Guide](CONTRIBUTING.md)
3. Open a new issue with detailed information

## Next Steps

After successful setup:

1. Explore the application features
2. Read the main [README.md](README.md)
3. Check out [CONTRIBUTING.md](CONTRIBUTING.md) if you want to contribute
4. Review the code in `src/components/SecureMedicalDataSharing.jsx`

Happy coding! 🚀
