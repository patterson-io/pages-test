# Pages Test - Next.js Starter Template

## Description

Pages Test is a Next.js starter template designed for learning and prototyping modern React applications. This repository serves as a foundation for building server-side rendered and statically generated web applications using Next.js framework. It's configured with automated deployment to GitHub Pages through GitHub Actions workflows, making it perfect for quickly setting up and deploying web projects.

The project includes a development container setup for consistent development environments and automated CI/CD pipelines for seamless deployment to GitHub Pages.

## Features

- **Next.js Framework**: Built with the latest Next.js for optimal performance and developer experience
- **React 17**: Modern React with hooks and functional components
- **Automated Deployment**: GitHub Actions workflows for continuous integration and deployment to GitHub Pages
- **Development Container**: Pre-configured VS Code dev container with Node.js environment
- **Static Site Generation**: Optimized for static exports suitable for GitHub Pages hosting
- **Responsive Design**: Mobile-first responsive layout with CSS-in-JS styling
- **Production Ready**: Optimized builds with automatic code splitting and performance optimizations

## Installation

### Prerequisites

- **Node.js**: Version 14.17.4 or higher (as specified in `.nvmrc`)
- **npm**: Comes bundled with Node.js
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

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser** and navigate to `http://localhost:3000`

### Development Container (Optional)

For a consistent development environment, you can use the included development container:

1. Open the project in Visual Studio Code
2. Install the "Remote - Containers" extension
3. Click "Reopen in Container" when prompted
4. The container will automatically set up Node.js, yarn, and other development tools

## Usage

### Development Commands

```bash
# Start development server with hot reload
npm run dev

# Build the application for production
npm run build

# Start the production server
npm run start
```

### Building for GitHub Pages

The project is configured to automatically build and deploy to GitHub Pages when code is pushed to the main branch. For manual deployment:

```bash
# Build and export static files
npm run build
npm run env -- next export -o build
```

### Code Examples

The main page component demonstrates basic Next.js features:

```javascript
import Head from 'next/head'

export default function Home() {
  return (
    <div className="container">
      <Head>
        <title>Create Next App</title>
        <link rel="icon" href="/favicon.ico" />
      </Head>
      
      <main>
        <h1 className="title">
          Welcome to <a href="https://nextjs.org">Next.js!</a>
        </h1>
        {/* Your content here */}
      </main>
    </div>
  )
}
```

## Repository Structure

```
├── .devcontainer/
│   ├── Dockerfile              # Development container configuration
│   └── setup.sh               # Container setup script with dev tools
├── .github/
│   └── workflows/
│       ├── build-deploy.yaml   # Main CI/CD workflow for GitHub Pages
│       └── stack-init.yaml     # Stack initialization workflow
├── pages/
│   └── index.js               # Main page component with styled layout
├── public/
│   ├── favicon.ico           # Site favicon
│   └── vercel.svg           # Vercel logo asset
├── .gitignore               # Git ignore patterns for Node.js projects
├── .nvmrc                   # Node.js version specification (v14.17.4)
├── package.json             # Project dependencies and scripts
├── package-lock.json        # Locked dependency versions
└── README.md               # This comprehensive documentation
```

### Key Directories and Files

- **`.devcontainer/`**: Contains Docker configuration for VS Code development containers
- **`.github/workflows/`**: GitHub Actions workflows for automated CI/CD
- **`pages/`**: Next.js pages directory - each file becomes a route
- **`public/`**: Static assets served directly by Next.js
- **`package.json`**: Defines project dependencies (Next.js, React, React-DOM)

## Contributing

We welcome contributions to improve this starter template! Here's how you can contribute:

### Getting Started

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Make your changes and test them thoroughly
4. Commit your changes: `git commit -m 'Add amazing feature'`
5. Push to the branch: `git push origin feature/amazing-feature`
6. Submit a Pull Request

### Development Guidelines

- Follow existing code style and formatting
- Test your changes locally using `npm run build`
- Ensure the application builds successfully for static export
- Update documentation for any new features or changes
- Keep commits focused and atomic

### Reporting Issues

If you encounter any issues or have suggestions for improvements:

1. Check existing issues to avoid duplicates
2. Create a new issue with a descriptive title
3. Include steps to reproduce the problem
4. Provide your environment details (Node.js version, OS, etc.)

### Code Review Process

All contributions go through code review:

1. Automated checks must pass (build, deploy workflow)
2. At least one maintainer review is required
3. Changes should not break existing functionality
4. Documentation should be updated accordingly

## License

This project does not currently specify a license. Please refer to the repository settings or contact the maintainers for licensing information.

## Acknowledgments

- **Next.js Team**: For creating an excellent React framework
- **Vercel**: For hosting and deployment infrastructure
- **React Team**: For the powerful component library
- **GitHub**: For providing free hosting via GitHub Pages
- **Learn Next.js Tutorial**: This template is based on the official Next.js learning resources

### Useful Resources

- [Next.js Documentation](https://nextjs.org/docs) - Comprehensive guides and API reference
- [Learn Next.js](https://nextjs.org/learn) - Interactive tutorial for beginners
- [React Documentation](https://reactjs.org/docs) - Official React documentation
- [GitHub Pages](https://pages.github.com/) - Free hosting for static sites

---

```
 _________________________________________________
< Thanks for checking out this Next.js project! >
 -------------------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```