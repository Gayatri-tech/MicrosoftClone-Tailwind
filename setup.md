## How to setup tailwind css

STEP 01: Create index.html and write boilerplate, then run the following command:

```
npm init -y
```

STEP 02: Install Tailwind CSS using:

```
npm install -D tailwindcss
npx tailwindcss init
```

STEP 03: Update tailwind.config.js file to include this line:

```
 content: ["*.html"],
```

STEP 04: Create src/input.css and add the following to input.css file:

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

STEP 05: Run

```
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

STEP 06: Include src/output.css file to your index.html file via link:css

```
 <link rel="stylesheet" href="./src/output.css" />
```

Note: I have made this above(STEP 05) command short by adding it to the package.json file by the name 'build', hence I can use it directly:

```
npm run build
```

To generate full configuration file, run the following command:

```
npx tailwindcss init fileName --full
```
