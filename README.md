# eslint-config

My ESLint config

---

Install the dependencies:

```
npm install --save-dev eslint husky @vietduc/eslint-config
```

Use this `.eslintrc.json` config file:

```JSON
{
    "extends": ["airbnb-base", "plugin:jest/recommended", "@vietduc"]
}
```

Use this `.huskyrc.json` config file to enforce ESLint rules before committing:

```JSON
{
    "hooks": {
        "pre-commit": "node_modules/.bin/eslint ."
    }
}
```
