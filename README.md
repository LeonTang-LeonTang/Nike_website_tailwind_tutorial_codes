# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

The error sh: vite: command not found occurs because vite is not installed or not properly recognized. Here’s how you can resolve the issue:

# 1. Install Vite:

Make sure that vite is installed as a dependency. You can install it by running:

```
npm install vite --save-dev
```

# 2. Verify vite in package.json:

Check if vite is listed in your package.json under devDependencies. If it’s missing, the above command will add it. If vite is already listed but still not recognized, try reinstalling your dependencies:

```
npm install
```

# 3. Check Local vs Global Installation:

Ensure you’re using a local installation of vite within your project. If you’ve installed vite globally, you can try installing it locally within the project instead:
```
npm install vite --save-dev
```
# 4. Clear npm Cache (Optional):

If you suspect a caching issue, you can clear the npm cache and then reinstall dependencies:
```
npm cache clean --force
npm install
```

# 5. Verify Installation:

After installing, check if vite is in the node_modules/.bin folder. This folder should contain the vite executable for local projects.

# 6. Try Running Again:

Once Vite is installed correctly, try running your development server again:
```
npm run dev
```
If you’re still encountering the issue, let me know, and we can explore additional solutions!
