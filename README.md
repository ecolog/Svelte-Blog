# Blog

This is a personal blog for writing about audio, music, and sound related topics.

The text content is stored on a separate github repository and the page makes a fetch request to the raw content api for the text file. The text is parsed and added to the DOM using a basic implementation of the CommonMark markdown standard. Read the CommonMark spec [here](https://spec.commonmark.org/0.29/)

The parser also adds basic styling to the elements that it creates. This way the content for the website can easily be edited or updated by anyone, and they do not necessarily need to be able to write html or css

# svelte-tailwindcss-template

This is a starter template using Svelte and TailwindCSS.

This template overwrites the default tailwindcss color palette with the material design color palette. The colors can be found and modified in materialPalette.js

tailwind is set up as a svelte preprocess. That means that on build all the tailwind classes are put into the bundle.css file. Consequently, Postcss is also installed and purgecss is used to remove unused classes.

This template also has autoprefixer which automatically adds vendor specific css prefixes.

tailwindcss-bg-alpha creates background color classes that also have alpha variants. You have to specify what colors to generate these classes for in the tailwind.config.js file

I also included svelte-media because it is so usefull for making mobile friendly svelte apps. I set up the default watchMedia store to use the tailwindcss breakpoints.

## Get started

Install the dependencies...

```bash
npm install
```

...then start [Rollup](https://rollupjs.org):

```bash
npm run dev
```

Navigate to [localhost:5000](http://localhost:5000). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.

By default, the server will only respond to requests from localhost. To allow connections from other computers, edit the `sirv` commands in package.json to include the option `--host 0.0.0.0`.
