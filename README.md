# Fleet Management System

A modern, comprehensive fleet management application built with React, TypeScript, and Material-UI. This system provides real-time tracking, trip management, and analytics for managing vehicle fleets efficiently.

## 🚀 Features

### Core Functionality
- **Dashboard**: Real-time fleet statistics, performance metrics, and data visualizations
- **Vehicle Management**: Track and manage fleet vehicles with detailed information
- **Driver Management**: Maintain driver profiles, licenses, and performance records
- **Trip Management**: Create, schedule, and monitor trips with route planning
- **Real-time Tracking**: Live vehicle location tracking and route monitoring
- **Analytics & Reports**: Comprehensive reporting on fleet performance and efficiency
- **Maintenance Scheduling**: Track vehicle maintenance and service records
- **Fuel Management**: Monitor fuel consumption and costs

### Technical Features
- **Google Maps Integration**: Location autocomplete and route planning with fallback support
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Real-time Updates**: Live data synchronization across the platform
- **Secure Authentication**: Session-based auth with YAML configuration
- **Offline Support**: Fallback systems work without external APIs

## 🛠️ Technology Stack

### Frontend
- **React 19.1** - Latest React with concurrent features
- **TypeScript 5.3** - Type-safe development
- **Material-UI v7** - Modern UI components
- **React Router v7** - Advanced routing
- **Recharts** - Data visualization
- **Framer Motion** - Smooth animations
- **Google Maps API** - Location services

### Architecture
- **Microservices Design** - Scalable service-oriented architecture
- **RESTful APIs** - Standard API communication
- **Component-based** - Reusable React components
- **State Management** - React hooks and context

## 📋 Prerequisites

- Node.js 18+ and npm 9+
- Google Maps API key (optional, for enhanced location features)
- Modern web browser

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/fleet-management-app.git
cd fleet-management-app
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Environment Setup (Optional)
For Google Maps integration, create a `.env.local` file:
```env
REACT_APP_GOOGLE_MAPS_API_KEY=YOUR_ACTUAL_GOOGLE_MAPS_API_KEY_HERE
```

### 4. Run the Application
```bash
npm start
```

The application will start on `http://localhost:3000` (or port 3002 if configured).

### 5. Demo Login Credentials ( Testing purpose )
```
Username: admin
Password: admin
```

## 📁 Project Structure

```
fleet-management-app/
├── public/
│   ├── index.html          # HTML template with Google Maps script
│   ├── settings.yaml       # Authentication configuration
│   └── assets/             # Static assets
├── src/
│   ├── components/         # Reusable UI components
│   │   ├── LocationAutocomplete/  # Google Maps autocomplete with fallback
│   │   ├── Login/          # Login page component
│   │   ├── Dashboard/      # Main dashboard component
│   │   └── common/         # Shared components
│   ├── pages/              # Page components
│   │   ├── Dashboard/      # Dashboard page
│   │   ├── Vehicles/       # Vehicle management
│   │   ├── Drivers/        # Driver management
│   │   ├── Trips/          # Trip management
│   │   ├── Analytics/      # Reports and analytics
│   │   └── Maintenance/    # Maintenance tracking
│   ├── services/           # API services
│   ├── data/              # Mock data and fallback databases
│   │   └── locations.ts    # 30+ common locations for offline support
│   ├── styles/            # Global styles and themes
│   ├── utils/             # Utility functions
│   └── App.tsx            # Main application component
├── docs/
│   ├── SolutionDesign.md   # System architecture and design
│   └── SETUP_GOOGLE_MAPS.md # Google Maps setup guide
└── package.json           # Project dependencies
```

## 🗺️ Google Maps Integration

The application includes advanced location features:

### With Google Maps API
- Real-time location autocomplete
- Precise address suggestions
- Automatic distance and duration calculation
- Current location detection

### Without Google Maps API (Fallback)
- 30+ pre-configured common locations
- Includes major airports, cities, and business districts
- Works completely offline
- Search by name, city, or state

See `SETUP_GOOGLE_MAPS.md` for detailed setup instructions.

## 🌟 Key Features Details

### Dashboard
- **Real-time Statistics**: Vehicle count, active trips, driver availability
- **Performance Metrics**: Fuel efficiency, trip completion rates
- **Visual Analytics**: Interactive charts using Recharts
- **Recent Activities**: Latest trips and events

### Trip Management
- **Multi-step Creation Process**:
  1. Select Vehicle
  2. Assign Driver
  3. Set Route Details (with location autocomplete)
  4. Schedule Trip
- **Route Planning**: Origin and destination with smart suggestions
- **Distance Calculation**: Automatic estimation based on selected route
- **Trip Tracking**: Real-time status updates

### Vehicle Management
- **Fleet Overview**: List all vehicles with status
- **Detailed Profiles**: Registration, type, maintenance history
- **Availability Tracking**: Real-time vehicle availability
- **Performance Metrics**: Individual vehicle statistics

### Driver Management
- **Driver Profiles**: Personal info, license details, experience
- **Assignment History**: Track driver assignments
- **Performance Tracking**: Driver efficiency metrics
- **Availability Status**: Real-time driver availability

## 🔧 Configuration

### Running on Different Ports
```bash
# Default port 3000
npm start

# Custom port
PORT=3002 npm start
```

### Environment Variables
- `REACT_APP_GOOGLE_MAPS_API_KEY`: Google Maps API key
- `PORT`: Application port (default: 3000)

## 🔒 Security Features

- Session-based authentication
- Secure API key handling
- Environment variable protection
- Input validation and sanitization
- CORS protection
- YAML-based user management (to be migrated to database)

## 🚧 Development

### Available Scripts

```bash
# Start development server
npm start

# Run tests
npm test

# Build for production
npm run build

# Run linting
npm run lint

# Type checking
npm run type-check
```

### Code Quality
- TypeScript strict mode enabled
- ESLint configuration
- Prettier for code formatting
- Component-based architecture
- Clean code principles

## 📈 Roadmap

### Phase 1 (Current)
- ✅ Modern UI with Material-UI
- ✅ Dashboard with analytics
- ✅ Basic authentication
- ✅ Trip creation with Google Maps
- ✅ Responsive design

### Phase 2 (Next)
- [ ] PostgreSQL database integration
- [ ] RESTful API implementation
- [ ] Real-time GPS tracking
- [ ] Advanced reporting
- [ ] Mobile app (React Native)

### Phase 3 (Future)
- [ ] Microservices architecture
- [ ] IoT device integration
- [ ] Predictive maintenance
- [ ] AI-powered route optimization
- [ ] Multi-tenant support

## 🎨 Design Principles

### UI/UX
- **Modern Design**: Clean, professional interface
- **Smooth Animations**: Framer Motion for interactions
- **Responsive**: Mobile-first approach
- **Accessibility**: WCAG compliant

### Architecture
- **Scalable**: Microservices-ready design
- **Maintainable**: Component-based structure
- **Testable**: Separated concerns
- **Extensible**: Plugin architecture

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is proprietary software owned by Fleet Solutions Inc.

## 👥 Team

- **Frontend Development**: React/TypeScript team
- **UI/UX Design**: Material-UI implementation
- **Backend Architecture**: Microservices design
- **DevOps**: CI/CD pipeline setup

## 📞 Support

For support and queries:
- Create an issue in the GitHub repository
- Contact the development team
- Check the documentation in `/docs`

## 🙏 Acknowledgments

- Material-UI for the component library
- Google Maps Platform for location services
- React team for the amazing framework
- All contributors and testers

---

**Note**: This is a pilot MVP project. The authentication is currently file-based (settings.yaml) and will be migrated to PostgreSQL in the production phase.
