# 🌺 Kollam Rangoli Generator

A specialized web application that generates authentic traditional Kerala kollam rangoli designs using AI. Built with React, TypeScript, and Tailwind CSS, this app preserves and celebrates the centuries-old art of Kerala floor decorations.

![Kollam Rangoli Generator](https://img.shields.io/badge/Kollam-Rangoli%20Generator-orange?style=for-the-badge&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

## ✨ Features

### 🚀 Core Functionality
- **Kollam Rangoli Generation**: Create authentic Kerala floor art designs with AI
- **Traditional Patterns**: Specialized in geometric patterns, floral motifs, and cultural symbols
- **Instant Download**: Save generated rangoli designs directly to your device
- **Design Regeneration**: Recreate designs with the same prompt for variations
- **Traditional Inspiration**: Get inspired with 20+ authentic Kerala rangoli prompts

### 🎨 Premium UI/UX
- **Kerala-Inspired Design**: Warm orange, red, and yellow color scheme reflecting traditional art
- **Dark/Light Mode**: Seamless theme switching with system preference detection
- **Smooth Animations**: Fluid transitions, hover effects, and micro-interactions
- **Responsive Layout**: Optimized for mobile, tablet, and desktop devices
- **Cultural Aesthetics**: Traditional Kerala-inspired gradients and cultural motifs

### 🔧 Technical Features
- **TypeScript**: Full type safety and enhanced developer experience
- **Context API**: Efficient state management for images and app settings
- **Specialized Prompts**: Enhanced prompts specifically for kollam rangoli generation
- **Performance Optimized**: Lazy loading, efficient re-renders, and optimized animations
- **Accessibility**: WCAG compliant with proper focus management and ARIA labels

## 🛠️ Tech Stack

- **Frontend**: React 18 + TypeScript
- **Styling**: Tailwind CSS with custom animations
- **API**: Clipdrop Text-to-Image API with kollam-specific enhancements
- **Build Tool**: Vite
- **Icons**: Lucide React
- **State Management**: React Context API

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ and npm/yarn
- Clipdrop API key from [clipdrop.co](https://clipdrop.co/apis/text-to-image)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/kollam-rangoli-generator.git
   cd kollam-rangoli-generator
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   ```
   
   Add your Clipdrop API key to `.env`:
   ```env
   VITE_CLIPDROP_API_KEY=your_clipdrop_api_key_here
   ```

4. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:5173`

## 🔑 API Setup

### Getting Your Clipdrop API Key

1. Visit [Clipdrop API](https://clipdrop.co/apis/text-to-image)
2. Sign up for an account
3. Navigate to your dashboard
4. Copy your API key
5. Add it to your `.env` file

### API Usage
The app automatically enhances prompts with kollam rangoli-specific keywords:
- Adds traditional Kerala kollam terminology and cultural context
- Includes geometric pattern specifications and color guidance
- Ensures authentic traditional design elements
- Implements rate limiting and request optimization

## 📁 Project Structure

```
src/
├── components/          # React components
│   ├── Header.tsx      # App header with theme toggle
│   ├── ImageGenerator.tsx  # Main generation interface
│   ├── ImageGrid.tsx   # Grid layout for generated images
│   └── ImageCard.tsx   # Individual image display component
├── context/            # React Context providers
│   └── AppContext.tsx  # Global app state management
├── services/           # API services
│   └── clipdropService.ts  # Clipdrop API integration
├── types/              # TypeScript type definitions
│   └── index.ts        # Shared interfaces and types
├── utils/              # Utility functions
│   └── prompts.ts      # Random prompt generation
├── App.tsx             # Main app component
├── main.tsx           # App entry point
└── index.css          # Global styles and animations
```

## 🎨 Customization

### Themes
The app uses a Kerala-inspired color palette with warm oranges, reds, and yellows. Customize colors in `tailwind.config.js`:

```javascript
theme: {
  extend: {
    colors: {
      primary: { /* orange tones */ },
      secondary: { /* red tones */ },
      accent: { /* yellow tones */ },
    }
  }
}
```

### Animations
Custom animations are defined in `src/index.css`. Add new animations:

```css
@keyframes yourAnimation {
  /* keyframes */
}

.your-animation {
  animation: yourAnimation 2s ease-in-out infinite;
}
```

### Prompts
Add new traditional kollam rangoli prompts in `src/utils/prompts.ts`:

```typescript
export const surprisePrompts = [
  "Traditional Kerala kollam design with your specific elements",
  // ... more traditional rangoli prompts
];
```

## 🚀 Deployment

### Build for Production
```bash
npm run build
# or
yarn build
```

### Deploy to Netlify
1. Build the project
2. Deploy the `dist` folder to Netlify
3. Set environment variables in Netlify dashboard

### Deploy to Vercel
1. Connect your GitHub repository
2. Set environment variables in Vercel dashboard
3. Deploy automatically on push

## 🔧 Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `VITE_CLIPDROP_API_KEY` | Your Clipdrop API key | Yes |

## 📱 Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Clipdrop](https://clipdrop.co/) for the amazing Text-to-Image API
- Traditional Kerala artisans who have preserved kollam rangoli art for centuries
- Kerala's rich cultural heritage and artistic traditions
- [Tailwind CSS](https://tailwindcss.com/) for the utility-first CSS framework
- [Lucide](https://lucide.dev/) for the beautiful icons
- [React](https://reactjs.org/) for the powerful UI library

## 📞 Support

If you have any questions or need help, please:
- Open an issue on GitHub
- Check the [documentation](https://clipdrop.co/apis/docs)
- Contact support at your-email@example.com

---

**Made with ❤️ for Kerala's Cultural Heritage**

*Preserving and celebrating traditional Kerala kollam rangoli art through modern AI technology.*