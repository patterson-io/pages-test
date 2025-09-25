# Pages Test

## Description

Pages Test is a Next.js-based web application designed for testing GitHub Pages deployments and CI/CD workflows. This repository serves as a demonstration and testing platform for automated build and deployment processes using GitHub Actions, specifically focusing on static site generation and deployment to GitHub Pages.

The project features a modern React-based frontend built with Next.js, complete with automated testing, build processes, and deployment pipelines. It's particularly useful for developers who want to understand how to set up continuous deployment for static sites or test GitHub Pages configurations.

## Features

- **Next.js Framework**: Modern React-based web application with server-side rendering capabilities
- **Static Site Generation**: Optimized for deployment as static HTML files
- **GitHub Actions Integration**: Automated CI/CD pipeline for testing and deployment
- **GitHub Pages Deployment**: Seamless deployment to GitHub Pages with custom workflows
- **Development Container**: Pre-configured dev container with Node.js and development tools
- **Responsive Design**: Clean, responsive UI with modern styling
- **Zero Configuration**: Ready-to-use setup with minimal configuration required

## Installation

### Prerequisites

- **Node.js**: Version 14.17.4 (as specified in `.nvmrc`)
- **npm**: Comes with Node.js installation
- **Git**: For version control

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/patterson-io/pages-test.git
   cd pages-test
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000) to see the application running.

### Using the Development Container

If you prefer to use the provided development container:

1. **Open in VS Code with Dev Containers extension**
2. **Reopen in Container** when prompted
3. The container will automatically set up the environment with all necessary tools

## Usage

### Development Commands

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start
```

### Deployment

The repository includes automated deployment workflows:

- **Automatic Deployment**: Pushes to the `main` branch trigger automatic builds and deployments
- **Manual Deployment**: Use the "Build and Deploy Pages Site" workflow for manual deployments
- **Stack Initialization**: Use the "provision stack build/ deploy for ghpages" workflow to set up a new deployment environment

### Example Usage

The application displays a welcome page with links to Next.js resources:

- Documentation and learning materials
- Example projects and templates
- Deployment guides and best practices

## Repository Structure

```
├── .devcontainer/           # Development container configuration
│   ├── Dockerfile          # Container setup with Ubuntu 18.04
│   └── setup.sh            # Environment setup script
├── .github/                # GitHub-specific configuration
│   └── workflows/          # CI/CD workflows
│       ├── build-deploy.yaml    # Main build and deploy pipeline
│       └── stack-init.yaml      # Stack initialization workflow
├── pages/                  # Next.js pages directory
│   └── index.js           # Main application page component
├── public/                 # Static assets
│   ├── favicon.ico        # Site favicon
│   └── vercel.svg         # Vercel logo asset
├── .gitignore             # Git ignore patterns
├── .nvmrc                 # Node.js version specification
├── package.json           # Project dependencies and scripts
├── package-lock.json      # Dependency lock file
└── README.md              # Project documentation
```

### Key Files and Directories

- **`pages/index.js`**: Main React component containing the welcome page UI
- **`.github/workflows/`**: Contains automated CI/CD pipelines for building and deploying
- **`.devcontainer/`**: Development environment configuration for containerized development
- **`package.json`**: Defines project dependencies (Next.js, React) and npm scripts
- **`.nvmrc`**: Specifies Node.js version (v14.17.4) for consistent development environment

## Contributing

We welcome contributions to improve this testing platform! Here's how to get started:

### How to Contribute

1. **Fork the repository**
   ```bash
   git fork https://github.com/patterson-io/pages-test.git
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**
   - Follow existing code style and conventions
   - Add tests for new functionality
   - Update documentation as needed

4. **Test your changes**
   ```bash
   npm run build
   npm start
   ```

5. **Commit and push**
   ```bash
   git commit -m "Add your descriptive commit message"
   git push origin feature/your-feature-name
   ```

6. **Submit a Pull Request**
   - Provide a clear description of your changes
   - Reference any related issues
   - Ensure all CI checks pass

### Development Guidelines

- **Code Style**: Follow existing JavaScript/React conventions
- **Testing**: Ensure builds complete successfully
- **Documentation**: Update README.md for significant changes
- **Commits**: Use clear, descriptive commit messages

## License

This project does not currently have a specified license. Please contact the repository maintainers for licensing information before using this code in production environments.

## Acknowledgments

- **Next.js Team**: For the excellent React framework
- **Vercel**: For hosting and deployment tools
- **GitHub Actions**: For CI/CD infrastructure
- **React Team**: For the foundational UI library

---

### Fun Fact 

```
 _________________________________________
< This repo tests more than your patience! >
 -----------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```