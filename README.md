# node-template

> Personal template for Node.js projects.

## Installation

1. Create a new repository from this template
2. Run `git clone {NEW_REPO_URL}`
3. Configure the template for your new project
   - Update `README.md`
   - Update `package.json`
   - Delete `.env.example` or rename to `.env`
4. Run `npm install` to install dependencies and Git hooks
5. Run `npm start` to start development server

**NOTE:** Run `git config core.filemode false` if your development environment causes problematic file permissions (e.g. WSL with mounted drives).

## Features

### Developer experience

| Purpose        | Package     | Config file          |
| -------------- | ----------- | -------------------- |
| Linting        | ESLint      | `.eslintrc.json`     |
| Formatting     | Prettier    | `.prettierrc.json`   |
| Git hooks      | Husky       | `.huskyrc.json`      |
| Lint runner    | lint-staged | `.lintstagedrc.json` |
| VS Code config |             | `jsconfig.json`      |

### Environment variables

- Secrets
  1. Create `.env` file in root directory (example: `.env.example`) or pass through npm scripts
  2. Access in code with `process.env.{VARIABLE}`

### npm scripts

| Command                      | Description                    |
| ---------------------------- | ------------------------------ |
| `npm run clean:node_modules` | Clean `node_modules` directory |
| `npm run format:check`       | Check for formatting issues    |
| `npm run format:fix`         | Fix formatting issues          |
| `npm run lint:check`         | Check for linting issues       |
| `npm run lint:fix`           | Fix linting issues             |
| `npm start`                  | Start development server       |

### Ignore files

- `.gitignore`
- `.eslintignore`
- `.prettierignore`

## Roadmap

- TypeScript
- Jest

## Notes

- Should work on Unix-like operating systems and WSL

## Resources

- [PM2](https://github.com/Unitech/pm2) — production process manager

## Contact

[Website](https://dusktrades.com) • [Twitter](https://twitter.com/dusktrades) • [Email](mailto:dusktrades@protonmail.com)

## License

MIT © [Dusk](https://dusktrades.com)
