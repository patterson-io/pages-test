# Next.js Starter Template

A clean, minimal Next.js starter template designed to help you kickstart your Next.js projects with best practices and a productive development environment.

## 🚀 Description

This repository provides a battle-tested Next.js starter template that includes all the essentials to get you building modern React applications quickly. Whether you're a beginner learning Next.js or an experienced developer starting a new project, this template offers a solid foundation with sensible defaults and a containerized development environment.

Built with the latest Next.js framework, this template leverages server-side rendering (SSR), static site generation (SSG), and API routes to create performant, SEO-friendly web applications.

## ✨ Features

- **⚡ Next.js Latest**: Harness the power of the latest Next.js framework with hybrid static & server rendering
- **⚛️ React 17**: Build with React 17.0.2 for robust component-based architecture
- **🎨 CSS-in-JS**: Styled JSX included for scoped styling out of the box
- **🐳 Dev Container**: Fully configured `.devcontainer` setup for consistent development environments
- **📦 Minimal Dependencies**: Lean dependency tree with only essential packages
- **🔧 Ready to Customize**: Clean structure that's easy to extend and customize
- **📱 Responsive Design**: Mobile-friendly default styling
- **🚢 Deployment Ready**: Optimized for deployment to Vercel, Netlify, or any Node.js hosting

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js**: v14.17.4 (specified in `.nmvrc` file) or higher
- **npm**: v6+ or **yarn**: v1.22+
- **Git**: For version control

> **Note**: Using [nvm](https://github.com/nvm-sh/nvm) (Node Version Manager) is recommended to manage Node.js versions.

## 🛠️ Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/pages-test.git
cd pages-test
```

### Install Dependencies

Using npm:
```bash
npm install
```

Using yarn:
```bash
yarn install
```

### Using the Correct Node Version

If you have nvm installed:
```bash
nvm use
```

This will automatically switch to Node.js v14.17.4 as specified in the `.nmvrc` file.

## 🎯 Usage

### Development Server

Start the development server with hot module replacement:

```bash
npm run dev
```

or

```bash
yarn dev
```

The application will be available at [http://localhost:3000](http://localhost:3000).

Open your browser and navigate to the URL to see your Next.js application running. Edit `pages/index.js` to see changes reflected in real-time.

### Production Build

Create an optimized production build:

```bash
npm run build
```

or

```bash
yarn build
```

This command generates an optimized version of your application ready for deployment.

### Start Production Server

After building, start the production server:

```bash
npm start
```

or

```bash
yarn start
```

The production server will run at [http://localhost:3000](http://localhost:3000).

## 🐳 Development Container Setup

This project includes a complete development container configuration for use with GitHub Codespaces, VS Code Remote - Containers, or any container-based development environment.

### Features

- Pre-configured Dockerfile with Node.js environment
- Zsh shell integration
- Recommended VS Code extensions:
  - Bracket Pair Colorizer
  - GitHub Actions support
  - GitLens
  - GitHub Pull Requests
  - Docker support
  - Live Share
  - VS Code Icons
  - IntelliCode

### Using with VS Code

1. Install the [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension
2. Open the project in VS Code
3. When prompted, click "Reopen in Container" or press `F1` and select "Remote-Containers: Reopen in Container"

### Using with GitHub Codespaces

1. Navigate to the repository on GitHub
2. Click the "Code" button
3. Select "Open with Codespaces"
4. Click "New codespace"

Your development environment will be automatically configured with all necessary tools and extensions.

## 📁 Repository Structure

```
pages-test/
├── .devcontainer/          # Development container configuration
│   ├── Dockerfile          # Container image definition
│   ├── devcontainer.json   # Dev container settings and extensions
│   └── setup.sh            # Container setup script
├── pages/                  # Next.js pages directory
│   └── index.js            # Home page component
├── public/                 # Static assets
│   ├── favicon.ico         # Site favicon
│   └── vercel.svg          # Vercel logo
├── .gitignore              # Git ignore rules
├── .nmvrc                  # Node version specification (v14.17.4)
├── package.json            # Project dependencies and scripts
├── package-lock.json       # Locked dependency versions
└── README.md               # This file
```

### Key Directories

- **`pages/`**: Contains your application pages. Each `.js` file becomes a route automatically
- **`public/`**: Static files served directly. Access files via `/filename.ext`
- **`.devcontainer/`**: Configuration for containerized development environments

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
   ```bash
   git clone https://github.com/yourusername/pages-test.git
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```

3. **Make your changes**
   - Write clean, readable code
   - Follow the existing code style
   - Test your changes thoroughly

4. **Commit your changes**
   ```bash
   git commit -m 'Add some amazing feature'
   ```

5. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```

6. **Open a Pull Request**

### Code Style

- Use meaningful variable and function names
- Keep components small and focused
- Add comments for complex logic
- Follow React and Next.js best practices

## 📝 License

This project is open source and available for educational and commercial purposes.

## 🙏 Acknowledgments

- **[Next.js](https://nextjs.org/)** - The React framework for production
- **[Vercel](https://vercel.com/)** - For hosting and deployment platform
- **[React](https://reactjs.org/)** - For the amazing UI library
- **Next.js Team** - For creating and maintaining this incredible framework
- **Community Contributors** - For continuous improvements and feedback

## 📚 Additional Resources

- [Next.js Documentation](https://nextjs.org/docs) - Learn about Next.js features and API
- [Next.js Learn](https://nextjs.org/learn) - Interactive Next.js tutorial
- [React Documentation](https://reactjs.org/docs) - Learn React fundamentals
- [Next.js Examples](https://github.com/vercel/next.js/tree/master/examples) - Example Next.js projects
- [Next.js GitHub](https://github.com/vercel/next.js) - Source code and issues

## 🐛 Troubleshooting

### Port Already in Use

If port 3000 is already in use, you can specify a different port:
```bash
npm run dev -- -p 3001
```

### Node Version Issues

Ensure you're using the correct Node.js version:
```bash
node -v  # Should output v14.17.4 or compatible version
```

### Dependencies Not Installing

Clear npm cache and try again:
```bash
npm cache clean --force
rm -rf node_modules package-lock.json
npm install
```

---

## 🎭 Developer Humor

```
 ______________________________________
/ Why do Next.js developers never get \
| lost?                                |
|                                      |
| Because they always know the next    |
\ route! 🗺️                            /
 --------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

**Happy Coding!** 🎉 May your builds be fast and your bugs be few!