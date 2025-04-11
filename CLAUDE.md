# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build & Development Commands
- Install dependencies: `yarn`
- Start development server: `yarn dev`
- Build for production: `yarn build`
- Format code: `yarn format`
- Lint: `yarn format-ci` 
- Run all tests: `yarn test`
- Run single test file: `NODE_ICU_DATA=node_modules/full-icu sharetribe-scripts test src/path/to/file.test.js`
- Run server tests: `yarn test-server`

## Coding Style Guidelines
- **Formatting**: Use Prettier with single quotes, trailing commas for ES5, and always wrap prose
- **Component Structure**: Follow React functional component patterns with hooks
- **CSS**: Use CSS Modules for component styling
- **Types**: Use PropTypes for component props validation
- **Naming**: Use camelCase for variables/functions, PascalCase for components/classes
- **Imports**: Group imports by: React core, libraries, components, styles
- **Error Handling**: Use utility functions from `src/util/errors.js` to check for specific API errors
- **Logging**: Use `src/util/log.js` for error logging and Sentry integration
- **File Organization**: Components should have their own directory with component file, CSS module, and tests