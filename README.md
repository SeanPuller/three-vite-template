# three-vite-template
todo: 
- update links
- setup example

# Webpage
https://pages.ghe.oculus-rep.com/Metaworks-Art/Threejs-Example/

# Development

### Comands to setup and run environment

Setup
```
npm install
```

Run
```
npm run dev
```

### Deploying website to github pages

Deploy
```
npm run deploy
```
### For creating a new project

Create
```
npm create vite
"vanilla"
npm install three
npm install lil-gui
npm install stats-js
npm install gh-pages --save-dev
```
Add a vite.config.js file with name of site. **Assets should be placed in the src folder**
```
export default {
    // config options
    base: 'https://pages.ghe.oculus-rep.com/Metaworks-Art/Threejs-Example/',
    assetsInclude: ['**/*.glb']
  }
  ```
Add lines to package.json
```
 "homepage": "https://pages.ghe.oculus-rep.com/Metaworks-Art/Threejs-Example/",
 
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d dist"
  },
```
