# Project Scripts

This repository contains several scripts to build and run an Electron application with react.

## Vite and Electron

Vite is a modern build tool that provides a fast and optimized development experience. Compared to other build tools like Create React App, Vite's unique features such as instant server start and lightning-fast hot module replacement make it a popular choice among web developers. Vite's ability to handle modern web technologies like ES modules, TypeScript, and CSS preprocessors allows you to write code that is easy to read, maintain, and scale.

When it comes to building desktop applications, Electron is a popular choice due to its ability to leverage web technologies to build cross-platform applications. By combining Vite and Electron, you can build desktop applications with a modern, optimized build process that leverages the latest web technologies.

Using Vite with Electron allows you to build desktop applications with a fast, optimized development experience. Vite's ability to handle modern web technologies and its optimized build process helps improve the performance of Electron applications, which can often be slow and resource-intensive. Additionally, Electron's cross-platform capabilities mean that you can build applications for Windows, macOS, and Linux with a single codebase.

In summary, Vite and Electron make a great combo for building fast and efficient desktop applications. By leveraging the strengths of both tools, you can create modern, optimized, and cross-platform applications with ease. If you're looking to build a desktop application, consider using Vite and Electron for a streamlined development experience.

## Scripts

- `dev`: Starts a development server using Vite.

- `build`: Builds the application using Vite.

- `lint`: Runs ESLint on the `src` directory to check for syntax errors and code style violations.

- `preview`: Starts a preview server using Vite to preview the built application.

- `esbuild-cjs`: Builds the `main.js` file using esbuild and outputs it in CommonJS format to the `./dist/main.cjs` file.

- `electron:dev`: Builds the `main.js` file using esbuild and starts the Electron application in development mode with the `IS_IN_DEVELOPMENT=true` environment variable set.

- `electron:build`: Builds the `main.js` file using esbuild and packages the Electron application for release using `electron-packager`.

### The esbuild-cjs Script

The `esbuild-cjs` script is used to build our ES modules to CommonJS format. It uses esbuild, a fast JavaScript bundler and minifier, to build the `main.js` file in CommonJS format and output it to the `./dist/main.cjs` file. This allows us to use the `main.cjs` file in our Electron application.

### The electron:dev and electron:build Scripts

The `electron:dev` and `electron:build` scripts are used to build and run our Electron application. Both scripts use the `esbuild-cjs` script to build the `main.js` file to CommonJS format.

The `electron:dev` script starts the Electron application in development mode with the `IS_IN_DEVELOPMENT=true` environment variable set.

The `electron:build` script packages the Electron application for release using `electron-packager`.

## Usage

To use these scripts, you must have Node.js and npm installed on your system. Clone this repository and run the scripts using npm, like so:

```bash

# Install dependencies

npm install



# Start development server

npm run  dev



# Build the application

npm run  build



# Preview the built application

npm run  preview



# Run ESLint

npm run  lint



# Build main.js in CommonJS format

npm run  esbuild-cjs



# Start Electron in development mode

npm run  electron:dev



# Build and package Electron application for release

npm run  electron:build

```

## Encouragements

If you find this repository useful, I encourage you to clone it and use it as a starting point for your own Electron application. You can customize the scripts and configuration files to fit your specific needs.

As an open-source project, contributions from the community are always welcome. If you have any feedback or suggestions for improvement, please feel free to submit an issue or pull request. Your contributions are greatly appreciated!

Thank you for considering this repository for your Electron application needs.

## License

This repository is licensed under the MIT License. See the `LICENSE` file for more details.# Project Scripts
