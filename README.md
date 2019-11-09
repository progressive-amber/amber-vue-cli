<img src="https://camo.githubusercontent.com/5b54cc5a749519515e15846ac911b094fa762ee5/687474703a2f2f7365616e776174746572732e696f2f696d616765732f616d6265722d7675652e706e67" alt="amber-vue" data-canonical-src="http://seanwatters.io/images/amber-vue.png" height="200">

<a href="https://amberframework.org/"><img src="https://img.shields.io/badge/using-amber_framework-orange.svg" ></a>
<a href="https://github.com/seanwatters/amber-vue/"><img src="https://img.shields.io/badge/using-amber_vue-green.svg" ></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-brightgreen.svg" ></a>

# Amber Vue.js CLI

This is a development tool for quickly scaffolding Amber apps using the [Amber Vue.js](https://github.com/seanwatters/amber-vue) recipe for the framework. 

## Installation

To run the **Amber Vue CLI**, you will need to have first created and Amber project using the **Amber with Vue** recipe.

```
amber new <project-name> -r seanwatters/amber-vue

cd <project-name>
```

From here, you will need to install the dependencies, including the **Amber Vue CLI**:

```
npm install
```

You can now use the tool. A script has been written into your projects, `package.json` file that will run the `node frontend-vue/dev/vue-tools.js` command for you.

```
npm run vue-tools

// alternatively
node vue-frontend/dev/vue-tools.js
```

## Usage

Now that the tool is installed, when you run `npm num react-tools`, you will be prompted with the following:

```
? Select Generator
> componenet
> scaffold
> api
```

Selecting `component` will prompt you to enter the component name, props and state. (state and props are not currently functional, but will be soon):

```
? Select Generator component
? Component Name: NewComponent
? Component State: <component-state>
? Component Props: <component-props>
```

This will generate a file in the `frontend-react/src/components/`:

```
|- frontent-react
    |- dev
    |- src
       |- components
           |- NewComponent.vue   // generated component
    |- index.css
    |- index.js
```

_keep in mind that this is not a substitution for [Vue.js devtools](https://github.com/vuejs/vue-devtools), but is a suplimental tool for development with **Amber with Vue**._

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
