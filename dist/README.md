# RHD Frontend Pattern Library

This is a test repo for the rhd-frontend project, delivered as an installable package on GitHub.

## Build process
```bash
  npm install
  gulp build
```

- `npm install`: install dependencies
- `gulp build`: builds the distributable code. Copies content from various locations into the `/dist` folder and includes the following:
  - package.json
  - README.md
  - css/rhd-theme/rhd-theme.css

### Additional build commands

- `gulp`: executes the CSS build command
- `gulp css`: the CSS build command. Runs the `.scss` code through autoprefixer, injects the package.json banner into the top of the file, creates a sourcemap, and drops folder into the appropriate location under the `./css` directory.
- `gulp copy-source`: Copy build files into the `./dist` directory. Runs the `clean-dist` command first to ensure that only the latest content is included.
- `gulp build`: Copy the files to the /dist location, running and completing the CSS build first.

## Requirements

To build this package locally (not accepting the prebuilt files we provide), you will need to have Node v10 and NPM v6.12 installed.
