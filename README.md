# Cursor Scaffolding

A modern, AI-compatible project template designed for seamless collaboration between developers and AI agents.

## 🚀 Features

- **AI-First Development**: Optimized for Cursor AI integration
- **TypeScript Support**: Full type safety across frontend and backend
- **Modern Stack**: React + Node.js with Express
- **Comprehensive Testing**: Unit, integration, and E2E testing setup
- **Documentation**: Detailed API and component documentation
- **Development Tools**: ESLint, Prettier, and Git hooks

## 📋 Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Git
- Cursor IDE

## 🛠️ Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/cursor-scaffolding.git
   cd cursor-scaffolding
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

4. **Start development servers**
   ```bash
   # Start backend
   npm run dev:backend
   
   # Start frontend
   npm run dev:frontend
   ```

## 📁 Project Structure

```
/project-root
├── .cursor/
│   └── rules/           # Cursor AI rules
├── src/
│   ├── frontend/        # React frontend
│   └── backend/         # Node.js backend
├── docs/               # Documentation
├── tests/              # Test files
└── cursor.json         # Cursor configuration
```

## 🧪 Testing

```bash
# Run all tests
npm test

# Run frontend tests
npm run test:frontend

# Run backend tests
npm run test:backend
```

## 📚 Documentation

- [API Documentation](./docs/api.md)
- [Component Library](./docs/components.md)
- [Architecture Decisions](./docs/architecture.md)
- [Development Guidelines](./docs/development.md)

## 🤖 Cursor AI Integration

This project is optimized for Cursor AI with:
- Project-specific rules in `.cursor/rules/`
- AI-friendly code structure
- Comprehensive documentation
- Clear component and API patterns

## 📝 Contributing

1. Create a feature branch
2. Make your changes
3. Run tests and linting
4. Submit a pull request

## 📄 License

MIT License - see [LICENSE](./LICENSE) for details 