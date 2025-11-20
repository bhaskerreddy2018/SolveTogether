```markdown
# Setting Up API Directory and Dependencies

## Create Directory
```bash
mkdir api
```

## Initialize npm Project
```bash
npm init
```

## Install Dependencies
```bash
# TypeScript
npm install typescript
npm install --save-dev @types/node
```

## Initialize TypeScript
```bash
npx tsc --init
```

## TypeScript Configuration
Create `tsconfig.json` with the following content:

```json
{
  "compilerOptions": {
    /* Output */
    "outDir": "./dist",
    "rootDir": "./src",

    /* Language and Environment */
    "target": "ES2020",
    "module": "CommonJS",

    /* Module Resolution */
    "moduleResolution": "node",
    "esModuleInterop": true,
    "allowSyntheticDefaultImports": true,
    "resolveJsonModule": true,

    /* Strictness */
    "strict": true,
    "forceConsistentCasingInFileNames": true,
    "noImplicitAny": false,

    /* Source Maps */
    "sourceMap": true,

    /* Node.js Types */
    "types": ["node"]
  },

  "include": ["src"],
  "exclude": ["node_modules", "dist"]
}
```

## Install Additional Dependencies

```bash
# Express
npm install express
npm install --save-dev @types/express

# Environment Variables
npm install dotenv
npm install --save-dev @types/dotenv

# MongoDB
npm install mongoose
npm install --save-dev @types/mongoose

# CORS
npm install cors
npm install --save-dev @types/cors
```