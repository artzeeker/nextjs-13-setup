# Next.js 13 setup

## Create project

- Open terminal and using command

    ```shell
    yarn create next-app
    ```

- Answer prompts like this

    ```shell
    What is your project named? <app-name>
    Would you like to use TypeScript with this project? No / <Yes>
    Would you like to use ESLint with this project? No / <Yes>
    Would you like to use Tailwind CSS with this project? No / <Yes>
    Would you like to use `src/` directory with this project? <No> / Yes
    Use App Router (recommended)? No / <Yes>
    Would you like to customize the default import alias? <No> / Yes
    ```

## Project configurations

- Append this script to `package.json` file at `scripts` section

    ```json
    "scripts": {
        "dev": "next dev",
        "build": "next build",
        "start": "next start",
        "lint": "next lint",
        "clean": "npx rimraf .next node_modules" // add this script
    },
    ```
