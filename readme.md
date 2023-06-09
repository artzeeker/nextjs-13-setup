# Next.js 13 setup

## Create project

- Open terminal and using command

    ```shell
    yarn create next-app
    ```

- Answer the prompts below

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

- Setup [Next.js Project Structure](https://nextjs.org/docs/getting-started/project-structure).

## Project convention

- Minimum width of html `body` tag should be 320 pixels. To do this just add TailwindCSS class `min-w-[320px]` to `body` tag in `/app/layout.tsx`.

- Maximum container should be 1,280 pixels and centered. To do this just add TailwindCSS class `max-w-screen-xl` and `mx-auto` to containers.

- Desktop resolution considerate to be 1,024 pixels width or more.

- Use `clamp` function for responsive design. Use [Clamp Calculator](https://www.marcbacon.com/tools/clamp-calculator/) for clamp calculation. Minimum viewport range should be **320 pixels** and Maximum viewport range should be **1,280 pixels**, then input min and max target values follow designer's XD file.

---

TIPs:
