# ⚡ TypeScript Starter for Node.js

A minimal boilerplate to quickly get started with TypeScript in a Node.js environment.

---

## 🛠️ Setup Instructions

### 1. Initialize the project

```bash
yarn init -y

### 2. Install TypeScript and Node.js types

```bash
yarn add typescript @types/node

### 3. Install development tools

```bash
yarn add -D ts-node

### 4. Initialize TypeScript configuration aka tsconfig.json

```bash
yarn tsc --init --rootDir ./ --outDir ./dist --esModuleInterop --lib "ES2019" --module commonjs --resolveJsonModule --noImplicitAny
This sets up a tsconfig.json with the following compiler options:

    rootDir: Source files location (./)

    outDir: Output for compiled JS (./dist)

    esModuleInterop: Enables default import style (import express from 'express')

    lib: Use modern JS features (ES2019)

    module: CommonJS (used in Node.js)

    resolveJsonModule: Allows importing .json files

    noImplicitAny: Enforces explicit typing for better type safety


### 5. Add Scripts in package.json

```bash
"scripts": {
  "dev": "ts-node src/index.ts",
  "build": "tsc",
  "start": "node dist/index.js"
}

your-project/
├── src/
│   └── index.ts
├── dist/
├── package.json
├── tsconfig.json
└── README.md





