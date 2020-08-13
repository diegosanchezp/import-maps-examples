# Import Maps Examples

Simple examples of [import maps](https://github.com/WICG/import-maps) using the polyfill [es-module-shims](https://github.com/guybedford/es-module-shims). These examples come from the [blog post](https://diegosanchezp.github.io/blog/import-maps), visit for better explanation.

The purpose of these examples is try to use [lit-element](https://lit-element.polymer-project.org/guide/start) and [@polymer/paper-button](https://www.npmjs.com/package/@polymer/paper-button) with bare module specifiers in the browser without a bundler.

## Get started
Dependencies can only be installed with yarn
`yarn install` 

The import-map.json file should be auto generated after installed dependencies, if not
`yarn run postinstall`

Generate the web_modules folder
`npx run snowpack`

To see the examples in the browser, run the scripts in `package.json`

## Notes
- @polymer/paper-button had to be installed as a development dependency, since it would have conflicts with [@import-maps/generate](https://www.npmjs.com/package/@import-maps/generate)

- If you run the script "serve-chrome", you'll need to have the flag "Experimental Productivity Features" enabled on chrome. Read the blog post to find how to.

Enjoy!
