# tailwindcss-template

For generating the corresponding styles and then writing them to a static CSS file

## Commands to run

First thing first, is to install the Tailwindcss dependency by running the command:

```json
npm install
```

or

```json
npm i
```

After running either of the above commands which mean the same, a `node_module` folder should be generated, but no need for you to bother yourself with it.

The next command to run is `npm start`.

> I just simplified the process, explanation for running `npm start` below

If you open the `package.json` file, you'll notice a script has been added as:

```json
{
  ...
  "scripts": {
    "start": "npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch"
  },
  ...
}
```

So there's no need to write the long script command anymore which is `npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch` but when you run `npm start`, it's equivalent.

From the script command `npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch`, take note of the input path and the output path.

The input path is where your CSS file is, which in this case is in the `src` folder, and the name of the CSS file is `input.css` that why we have `./src/input.css`

`-o` means output

Now for the output path, `./dist/output.css`

`--watch` means to keep watch in the input css file for changes

Lastly the path to the HTML file is `/src/index.html`
