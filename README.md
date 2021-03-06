```
yarn install
```

Now build the extension using

```
yarn build
```

You will see a `build` folder generated inside `[PROJECT_HOME]`

To avoid running `yarn build` after updating any file, you can run

```
yarn watch
```

which listens to any local file changes, and rebuilds automatically.

## Adding React app extension to Chrome

In Chrome browser, go to chrome://extensions page and switch on developer mode. This enables the ability to locally install a Chrome extension.
Now click on the `LOAD UNPACKED` and browse to `[PROJECT_HOME]\build` ,This will install the React app as a Chrome extension.
When you go to any website and click on extension icon, injected page will toggle.

## Using SASS

Boilerplate contains [sass-loader](https://github.com/webpack-contrib/sass-loader), so you can use SASS instead of pure CSS in your project. To do so:

1. Rename `src/App.css` file to `src/App.scss`
2. Change import line in `src/app.js` from
   `import './App.css';` to `import './App.scss';`

## License

The repo is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
