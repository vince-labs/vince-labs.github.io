# Vince Labs GitHub Pages (`vince-labs.github.io`)

This repository contains the source code for the Vince Labs GitHub Pages website. It is a static website built to showcase projects, documentation, or other content related to Vince Labs.

## 🛠️ Technology Stack

- **Framework**: [Astro](https://astro.build/) (v6.1.1 or higher)
- **Environment**: [Node.js](https://nodejs.org/) (>= 22.12.0)
- **Package Manager**: NPM

## 🏗️ Project Architecture

The project is structured as a modern static site using Astro. It leverages file-based routing and minimal client-side JavaScript by default, ensuring fast loading times and a good developer experience. The repository is continuously deployed to GitHub Pages via GitHub Actions.

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Node.js (version 22.12.0 or higher)
- npm (Node Package Manager)

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/vince-labs/vince-labs.github.io.git
   ```
2. Navigate into the project directory:
   ```sh
   cd vince-labs.github.io
   ```
3. Install the required dependencies:
   ```sh
   npm install
   ```

### Running Locally

To start the local development server:

```sh
npm run dev
```

The site will be available at `http://localhost:4321`.

## 📂 Project Structure

A brief overview of the generated folder structure:

```text
/
├── public/           # Static assets (images, fonts, etc.) that skip the build process
├── src/              # Source code of the application
│   ├── assets/       # Processed assets
│   ├── components/   # Reusable UI components (Astro, React, Vue, etc.)
│   ├── layouts/      # Page layout templates
│   └── pages/        # File-based routing (pages and API endpoints)
├── .github/workflows/# GitHub Actions deployment workflows
├── package.json      # Project dependencies and npm scripts
└── astro.config.mjs  # Astro framework configuration
```

## ✨ Key Features

- **Fast by Default**: Built with Astro's Zero-JS frontend architecture.
- **Component-based**: Easy to maintain and expand using Astro components.
- **Automated Deployments**: Integrated with GitHub Actions for seamless deployment to GitHub Pages.

## 🔄 Development Workflow

1. **Development**: Create feature branches off `main` for new developments.
2. **Build**: Run `npm run build` to generate the static site output locally (into the `./dist` folder).
3. **Deployment**: Pushing any changes to the `main` branch automatically triggers the `Deploy to GitHub Pages` GitHub Action workflow (`.github/workflows/deploy.yml`). The workflow builds the site and deploys the `./dist` folder to GitHub Pages.

## 📝 Coding Standards

- Use ES Modules (`"type": "module"` is specified in `package.json`).
- Manage dependencies through `npm`. Ensure `package-lock.json` is committed.
- Component architecture should lean towards Astro's default behavior, minimizing client-side hydration unless necessary.

## 🧪 Testing

There is currently no formal unit testing framework configured in this repository. Ensure that local builds (`npm run build`) and previews (`npm run preview`) succeed before pushing to `main`.

## 🤝 Contributing

1. Fork the project.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## 📄 License

This project does not currently specify an explicit open-source license.
