# My Tailwind HTML Project

This is a simple project using Tailwind CSS with a static HTML file.

## Prerequisites
- [Node.js](https://nodejs.org/) installed
- [pnpm](https://pnpm.io/) installed (or use npm/yarn)

## Setup

1. **Install dependencies**

   If you haven't already, install Tailwind CSS as a dev dependency:
   ```sh
   pnpm add -D tailwindcss
   ```
   Or with npm:
   ```sh
   npm install -D tailwindcss
   ```

## Development

### Start Tailwind in Watch Mode

To automatically build your CSS as you develop, use the following command:

```sh
pnpm dev
```

This runs the script defined in your `package.json`:

```json
"dev": "npx @tailwindcss/cli -i ./src/input.css -o ./dist/output.css --watch"
```

This command:
- Uses the Tailwind CLI to process your CSS.
- Watches for changes in your source files.
- Outputs the generated CSS to `dist/output.css`.
- Automatically rebuilds the CSS whenever you save changes.

### Open HTML with Live Server

You can use the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) VS Code extension to serve your HTML file and see changes live.

1. Install the Live Server extension in VS Code.
2. Right-click your HTML file (e.g., `index.htm`) and select **"Open with Live Server"**.
3. Your browser will open the file and auto-refresh on changes.

## Project Structure
```
my-tailwind-html/
├── dist/
│   └── output.css
├── package.json
├── pnpm-lock.yaml
├── src/
│   ├── input.css
│   └── index.html
```

## Troubleshooting
- If styles do not appear, make sure `output.css` is being generated and linked correctly in your HTML.
- If you see MIME type errors, ensure your server is serving the correct file and path.

# html-tailwind-learn
