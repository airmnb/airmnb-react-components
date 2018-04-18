# AIRMNB React UI components
Building UI component libaray,borrowing some of the concepts from Brad Frost’s [Atomic Design](http://bradfrost.com/blog/post/atomic-web-design/). Brad breaks down web UI into 5 distinct parts: atoms, molecules, organisms, templates, and pages.

Our library will consist of atoms and molecules. This will allow us to quickly build our organisms, templates, and pages. in the dependant projects.

##Atoms -> Elements
Atoms are basically the smallest indivisible bits of UI. Think of buttons, links, inputs, etc, we’ll call them “elements".

##Molecules -> Components
Molecules are simple and distinct combinations of atoms. Going forward we’ll call these “components”. The word “component” is very natural for the React world, but we’ll be using it in a specific way. An example would be a search field, which is a combination of a label, an input, and a button. Another example would be a dropdown list, which consists of a button (to toggle the dropdown) a list, and list items.

##Getting Started
To setup the project in you local machine:
```
git clone https://github.com/airmnb/airmnb-react-components.git
git checkout master
npm i
```
Run `npm link` to create a symlink of our library locally, and run `npm link airmnb-react-components` in all dependant projects to tell them that we want to use that symlinked library.

##Development
1. run `npm run build` to build the project.
2. run `npm run build:watch` to watch the project and rebuild the project.
3. run `npm run lint` to validate the code.
4. run `npm run lint:watch` to watch the project and revalidate the project.
5. run `npm run prepublish`, to prepublish the project, it is just an alias to build