# Template vite react typescript

Opinionated, really minimal, project template to use vite with react, typescript, eslint and prettier.

This template have the minimal tools and defaults configurations, so you can easily change/adapt/extend to your needs.

Husky and lint-stage are include and configured to trigger when someone try to commit against the repository, to lint and enforces a code style/format according to eslint and prettier configuration (which you can change to your needs).

I really recommend configure your IDE/editor to use eslint and prettier to preview how the code style is apply before commit.

## INSTALL:
**Important**: Setup husky will fail if you not install dependencies and init the repository before. 

1. Get the template 🡇:

```bash
npx degit https://github.com/lensanag/Template-vite-react-typescript project-name && cd project-name
```

2. Init git repository 🐙:

```bash
git init
```

3. Install dependencies 📦:

```bash
npm install
```

4. Setup husky 🐶:

```bash
npm run prepare
```

5. Stage all files ➕:
```bash
git add .
```

6. Commit changes ⚡:

```bash
git commit -m 'startup project'
```

Now you've got a new brand project 💯 configured to use with:

- vite (as bundler)
- typescript
- react
- eslint
- prettier

## NOTES:

- Just replace to equivalent command of your favorite package manager if you don't want to use npm (I personally prefer 'pnpm' 😎; if this is your case, be sure 'pnpm' is set to install peer dependencies automatically)
- If you need avoid husky runs on CI environments: install the package 'if-ci' and update the property **scripts.prepare** on *package.json*:
```json
"scripts": {
...
"prepare": "if-ci || husky install"
...
}
```

## IMPORTANT

- You've got to take care with outdated packages. Run npm audit for your security issues:

```bash
npm audit
```

Thats all folks! Have a happy coding! 😊
