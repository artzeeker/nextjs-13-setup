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

- Append `clean` script to `package.json` file at `scripts` section

    ```json
    "scripts": {
        "dev": "next dev",
        "build": "next build",
        "start": "next start",
        "lint": "next lint",

        // Add this script to clean up your project for a clean install.
        "clean": "npx rimraf .next node_modules"
    },
    ```

## Project convention

soon

---

TIPs:

- min width of html `body` tag should be 320px

- desktop size considerate to be 1024px or more
