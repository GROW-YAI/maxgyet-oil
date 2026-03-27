# Maxgyet Oil Website

## Project Overview

Maxgyet Oil is a modern web application built for an oil and gas company. The website provides information about the company's services, products, and operations in the energy sector. 

### Main Features
- **Company Information**: Showcases the company's mission, vision, and values in the oil and gas industry
- **Services Display**: Presents the range of services offered by Maxgyet Oil
- **Responsive Design**: Fully responsive layout that works seamlessly on desktop, tablet, and mobile devices
- **Accessibility**: Integrated with the Boafo accessibility widget to ensure the site is accessible to all users, including those with disabilities

### Technologies Used
- **React 18**: Modern JavaScript library for building user interfaces
- **TypeScript**: Type-safe JavaScript for better code quality
- **Vite**: Fast build tool and development server
- **Tailwind CSS**: Utility-first CSS framework for rapid UI development
- **React Router**: Client-side routing for single-page application navigation
- **Boafo Accessibility Widget**: Third-party accessibility solution to enhance user experience

### Accessibility Integration
This project uses the [Boafo Accessibility Widget](https://boafo.co) to make the website accessible to all users. The widget provides features such as:
- Screen reader compatibility
- Keyboard navigation support
- High contrast modes
- Font size adjustments
- And more accessibility features

## How to Get Your Boafo API Key

To use the Boafo accessibility widget, you need to obtain an API key:

1. Visit [boafo.co](https://boafo.co)
2. Register for an account or log in to your existing account
3. Navigate to your dashboard
4. Copy your API key from the dashboard

## How to Integrate the Boafo Widget

For detailed integration instructions, please refer to the official integration guide:
[Boafo Widget Integration Guide](https://drive.google.com/file/d/1tvwK-sBZI2a4uldd6z5LD1iLblSl3WbG/view?usp=sharing)

## Setup Instructions

### Prerequisites
- Node.js (version 16 or higher)
- npm or yarn package manager

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/GROW-YAI/maxgyet-oil.git
   cd maxgyet-oil
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   ```
   
   Open the `.env` file and replace `your_boafo_api_key_here` with your actual Boafo API key:
   ```
   VITE_BOAFO_API_KEY=your_actual_api_key_here
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Open the application**
   Navigate to `http://localhost:3000` in your browser

### Building for Production

To create a production build:
```bash
npm run build
```

The built files will be in the `dist` directory.

## Project Structure

```
maxgyet-oil/
├── app/                    # Application source code
│   ├── components/         # React components
│   │   └── BoafoWidgetInitializer.tsx
│   ├── layout.tsx         # Root layout component
│   └── globals.css        # Global styles
├── src/                   # Additional source files
│   ├── components/        # Shared components
│   ├── layouts/           # Layout components
│   ├── pages/             # Page components
│   └── vite-env.d.ts     # TypeScript declarations
├── public/                # Static assets
├── .env                   # Environment variables (not committed)
├── .env.example           # Environment variable template
├── .gitignore            # Git ignore rules
├── package.json          # Project dependencies
├── tailwind.config.js    # Tailwind CSS configuration
├── tsconfig.json         # TypeScript configuration
└── vite.config.js        # Vite configuration
```

## Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `VITE_BOAFO_API_KEY` | Your Boafo accessibility widget API key | Yes |

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is proprietary and confidential. All rights reserved.

## Contact

For questions or support, please contact the development team.