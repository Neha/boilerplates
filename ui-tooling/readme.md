# UI Tools

UI toolings helps UI dev to automate the mundant tasks to the tools, and extensions.
We can divide the tools into 3 parts:

1. Linters, and formatters

2. Task runners

3. Bundlers

## Formatters

One of the most popular formatter is "prettier" - prettier can be implemented by the extension and across code-project. Formatters helps in formtting the content and bringing the conistsency in the code base.

[Prettier](https://prettier.io/)

### Steps to have eslint in your project:

1. Create a file .prettier.json

2. Install the npm `npm i prettier --save-dev`

3. Create the basic config file:

```JAVASCRIPT
{
  "singleQuote": true,
  "--no-bracket-spacing": true,
  "--tab-width": 4,
  "--no-semi": true,
  "overrides": [
    {
      "files": ["*.html", "*.css", "*.scss"],
      "options": {
        "singleQuote": false
      }
    }
  ]
}

```

4. In `overrides`, we can mention the files we want the prettier to ignore, and which rules to override. Eg: in above example prettier will ignore all HTML, CSS, SCSS files for the rule "singleQuote".

5. Install the extension - prettier

6. Go to VSCode settings, and do the following changes:

   a. Search format, select "Format on Save"

   b. Select default format - prettier

[Video Demo]()

Woah!! congrats you got your first formatter is setup.

## Linters

Linters helps in enforcing the code guidlines and automate lot of low tasks such as - keeping the external imports on the top of file.

Popular linter: [ESLint](https://eslint.org/)

### Steps to have ESLint in your project:

1. Install `npm init @eslint/config`

2. We will use eslint cli and it will create eslint config for us

3. To disable or override the rules we can add inside the `rules`

4. To ignore the files, we can add the files inside the `ignorePatterns`

[Video Demo]()

Woah!! congrats you got your first formatter is setup.
