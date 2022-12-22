**[Manage](https://rajanchaudhari08.github.io/manage/)** (Landing Page)

### Technologies used:

1. **HTML5**
2. **CSS3**
3. **[TailwindCSS](https://tailwindcss.com/)**
4. **JavaScript**

### Download & Install Editor, Application & Dependencies:
1. [VSCode](https://code.visualstudio.com/)
2. [NodeJS](https://nodejs.org/en/)
3. [TailwindCSS](https://tailwindcss.com/docs/installation)
    * **Tailwind CLI** (Prefer for Production)
    * Using PostCSS
    * Framework Guides
    * Play CDN

<p>TailwindCSS dependency</p>

```bash
npx init -y
npm npm install -D tailwindcss 
```

<p>Add path to output.css file</p>

_package.json file:_

```json
"scripts": {
    "build": "tailwindcss -i ./input.css -o ./css/main.css",
    "watch": "tailwindcss -i ./input.css -o ./css/main.css --watch"
  },
```

<p>Build, Compile input.css File & Watch output.css File</p>

```bash
npm run build
npm run watch
```
<p>Create TailwindCSS config file</p>

```bash
npx tailwindcss init
```
_tailwind.config.js_

* content

```javascript
content: ['./*.html'],
```
* theme

```javascript
screens: {
      sm: '480px',
      md: '768px',
      lg: '976px',
      xl: '1440px'
    },

extend: {
    colors: {
    brightRed: 'hsl(12, 88%, 59%)',
    brightRedLight: 'hsl(12, 88%, 69%)',
    brightRedSupLight: 'hsl(12, 88%, 95%)',
    darkBlue: 'hsl(228, 39%, 23%)',
    darkGrayishBlue: 'hsl(237, 12%, 61%)',
    veryDarkBlue: 'hsl(233, 12%, 13%)',
    veryPaleRed: 'hsl(13, 100%, 96%)',
    veryLightGray: 'hsl(0, 0%, 98%)',
    }
    },
```
<p>Insert link for CSS & JavaScript File in HTML File</p>

* Header

```html
<link rel="stylesheet" href="css/main.css">
```

* Body

```html
<script src="js/script.js"></script>
```

**Exclude** directory: _node_modules_ before pushing files and directories to main branch repository. Add directory: _node_modules_ in _.gitignore_ file.

Reference Links: [Tailwind UI](https://tailwindui.com/)
