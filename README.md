# Lockfile Parser

The Lockfile Parser is a Node.js-based tool designed to extract version resolutions from lockfiles and transform them into JSON format for easy readability and further processing within a Node.js environment or other systems.

Supported lockfiles:

- ✅ **yarn.lock**
- ❌ **pnpm-lock.yaml** _(work in progress)_
- ❌ **package-lock.json** _(work in progress)_

## Installation / Setting up

#### pnpm

You can install pnpm by running:

```bash
npm install -g pnpm@latest
```

This will install the latest version of pnpm on your machine globally.

#### dependencies

Install the project dependencies by running `pnpm install`.

#### environment

Copy the `.env.example` file found in the root folder of the project, rename it to `.env`, this will contain your secrets and protect from becoming a commit in version control, change all the variable key/value pairs to match your environment.

## How to use

1. Place the lockfile you wish to parse in the `src/input` directory.
2. Run the program using either `pnpm build && pnpm start` or `pnpm dev`.
3. Upon completion, retrieve the generated JSON file from the `src/output` folder.
4. Explore the extracted version resolutions conveniently structured in JSON format.
