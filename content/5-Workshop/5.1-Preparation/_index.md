---
title: "Setting up Development Environment"
weight: 1
chapter: false
pre: " <b> 5.1. </b> "
---

### 1. Prerequisites

To develop modern web applications, you need the following standard tools:

*   **Node.js (LTS Version):** Runtime environment for JavaScript/TypeScript.
*   **Git:** Distributed version control system.
*   **IDE:** Visual Studio Code (recommended).

**Recommended VS Code Extensions:**
*   **ESLint & Prettier:** Automate formatting and linting.
*   **Tailwind CSS IntelliSense:** Rapid Tailwind class suggestions.
*   **ES7+ React/Redux/React-Native snippets:** Code faster with shortcuts.

### 2. Initialize Next.js Project

We will use **Next.js** - the most popular React Framework today.

Run initialization command:

```bash
npx create-next-app@latest my-serverless-app
```

Detailed Configuration:
*   TypeScript: **Yes** (Type safety)
*   Tailwind CSS: **Yes** (Rapid styling)
*   ESLint: **Yes** (Linting)
*   App Router: **Yes** (Latest routing architecture)
*   Import Alias: **@/** (Cleaner imports)

### 3. Standard Project Structure

A scientific folder structure helps with future maintenance:

![VS Code Project Structure](/images/vscode_project_structure_1764662831690.png)

*   `src/app`: Contains Pages and Layouts (App Router).
*   `src/components`: Contains reusable UI Components (Button, Card...).
*   `src/hooks`: Contains Custom Hooks (useAuth, useChat...).
*   `src/lib`: Contains utility functions and configurations (AWS config).

### 4. Configure `tsconfig.json` (Best Practices)

To ensure strict TypeScript coding, update `tsconfig.json`:

```json
{
  "compilerOptions": {
    "target": "es5",
    "lib": ["dom", "dom.iterable", "esnext"],
    "allowJs": true,
    "skipLibCheck": true,
    "strict": true, // Important: Enable strict mode
    "forceConsistentCasingInFileNames": true,
    "noEmit": true,
    "esModuleInterop": true,
    "module": "esnext",
    "moduleResolution": "node",
    "resolveJsonModule": true,
    "isolatedModules": true,
    "jsx": "preserve",
    "incremental": true,
    "plugins": [
      {
        "name": "next"
      }
    ],
    "paths": {
      "@/*": ["./src/*"]
    }
  },
  "include": ["next-env.d.ts", "**/*.ts", "**/*.tsx", ".next/types/**/*.ts"],
  "exclude": ["node_modules"]
}
```

### 5. Install UI Libraries

```bash
cd my-serverless-app
npm install framer-motion lucide-react clsx tailwind-merge
```

### 6. Configure TailwindCSS

Set up CSS Variables in `tailwind.config.ts` to ensure Design System consistency.

```typescript
// tailwind.config.ts
import type { Config } from "tailwindcss";

const config: Config = {
  content: [
    "./src/pages/**/*.{js,ts,jsx,tsx,mdx}",
    "./src/components/**/*.{js,ts,jsx,tsx,mdx}",
    "./src/app/**/*.{js,ts,jsx,tsx,mdx}",
  ],
  theme: {
    extend: {
      colors: {
        primary: "#432c7a", // Primary color
        secondary: "#764ba2",
        accent: "#ffd700",
        background: "#1a0b2e", // Dark background
      },
      backgroundImage: {
        "gradient-radial": "radial-gradient(var(--tw-gradient-stops))",
      },
    },
  },
  plugins: [],
};
export default config;
```

---

### My Experience

{{% notice note %}}
**Why TypeScript?**
When I first started, I found TypeScript annoying because of all the red errors. But as the project grew, those errors saved me from dozens of silly bugs (like typos, wrong data types).
**Advice:** Enable `strict: true` from the start. "Short term pain, long term gain"!
{{% /notice %}}

### Verification & Testing

To ensure the environment is ready, perform the following checks:

**Test Case 1: Check Node.js Version**
Open terminal and run:
```bash
node -v
```
*Expected Result:* `v18.x.x` or higher (LTS).

**Test Case 2: Run Development Server**
```bash
npm run dev
```
*Expected Result:* Terminal shows:
```
ready - started server on 0.0.0.0:3000, url: http://localhost:3000
event - compiled client and server successfully in 1234 ms (150 modules)
```
Access browser and see the spinning Next.js logo!
