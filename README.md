# stylelint-scss-config
This is the common settings about [stylelint](https://github.com/stylelint/stylelint) for scss.

---

The rules include [stylelint-order](https://github.com/hudochenkov/stylelint-order/tree/master/rules/order), you can easily to order scss properties by stylelint with `--fix`.

## Run Sample

```bash
git clone https://github.com/explooosion/stylelint-scss-config.git
```

```bash
yarn # or npm install
```

```bash
yarn lint # or npm run lint
```

```bash
yarn lint:fix # with auto fix
```


## How To Use

### 1. Installation

Checkout the package.json and install the devDependencies.

#### npm 

```bash
npm install -D stylelint stylelint-config-prettier stylelint-config-sass-guidelines stylelint-config-standard stylelint-order stylelint-scss 
```

#### yarn

```bash
yarn add -D stylelint stylelint-config-prettier stylelint-config-sass-guidelines stylelint-config-standard stylelint-order stylelint-scss 
```

### 2. Add Scripts and Precommit

Please add the following script to package.json.

```json
{
 "scripts": {
    "lint": "stylelint app/scss/**/**/**/*.scss --syntax scss",
    "lint:fix": "stylelint app/scss/**/**/**/*.scss --syntax scss --fix"
  },
  "pre-commit": [
    "lint"
  ],
}
```

### 3. Add .stylelintrc.json

Copy `.stylelintrc.json` into project root directory.

### 4. Install extensions

If your IDE is [vscode](https://code.visualstudio.com/), please install the following extensions:

- [stylelint](https://marketplace.visualstudio.com/items?itemName=shinnn.stylelint)
- [vscode-stylefmt](https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-stylefmt)
- [EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)

### 5. Start Lint

Now you can check your scss with the following command:

```bash
yarn lint
```

## License

[MIT](http://opensource.org/licenses/MIT)