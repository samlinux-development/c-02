# c-02; Master Deployments of Static Websites on the Internet Computer

This is a sample project used to demonstrates how to deploy a static website to the Internet Computer using the [DFINITY Canister SDK](https://sdk.dfinity.org/docs/quickstart/local-quickstart.html).

This project is part of the icAcademy course [Master Deployments of Static Websites on the Internet Computer](https://icacademy.at/6513c18b1f66192cab8beb29).

All data can be changed and adjusted via the data.json file in root of this project.

This is an Astro project. For more information about Astro, visit the [Astro website](https://astro.build/).

The project uses the [Tailwind CSS](https://tailwindcss.com/) framework and a custom font. For more information see package.json.


## Prerequisites
To use this Astro project you need to install all dependencies first. To do so, run the following command in the root of this project:

**Note:** To get a clean git repository, a tool called `digit` is used. [degit](https://github.com/Rich-Harris/degit) makes a copy of the git repositorie.  Make sure you have it installed. If you haven't installed it yet, you can do so using the following command.

```bash
npm install -g degit
```

### Check Node.js version, Node.js > 18 is required
```bash
node -v
```
If you don't have Node.js installed, you can install it using the following command:
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
nvm install 18
```

### Check dfx version
```bash
dfx --version
```

If you don't have the DFINITY Canister SDK installed, you can install it using the following command:

```bash
sh -ci "$(curl -fsSL https://internetcomputer.org/install.sh)"
```

## Installation steps

```bash
mkdir myapp && cd myapp
```

```bash
npx degit https://github.com/samlinux-development/c-02
```

```bash
npm install
```

```bash
dfx start --clean --background
```

```bash
# deploy to local replica
dfx deploy
```

```bash
# deploy to Motoko playground
dfx deploy --playground
```

```bash
echo http://$(dfx canister id c-02).localhost:4943
```

## Start the dev server
To start the local dev server, run the following command in the root of this project:

```bash
npm run dev
```

## Build the project
To build the project, run the following command in the root of this project:

```bash
npm run build
```
