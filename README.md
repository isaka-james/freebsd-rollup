# freebsd-rollup.sh 🚀

Yo, FreeBSD gang! Tired of dealing with that annoying native dependency crap when you're trying to build your React, Angular, or whatever the framework flavor of the month is?

Fear no more! I've cooked up a little magic called **`freebsd-rollup.sh`**. This script is built to **handle Rollup** like a boss on FreeBSD, so you can get back to coding without headaches.

## Why Should You Care? 🤔

Because it's 2024, and dealing with platform-specific build problems is lame! FreeBSD users often get left out in the cold with native builds, but not anymore. Thanks to the **@rollup/wasm-node** package, we bypass that native nonsense and let you keep grinding without worrying about dependency pain.

## How It Works 🛠️

This script installs the **@rollup/wasm-node** module and patches the native Rollup config to make your FreeBSD project just work™️ with frameworks like:

- **React** ⚛️  
- **Angular** 🅰️  
- **Vue** 🌲  
- And any other front-end framework you throw at it 🔥

You just **run this bad boy once**, and you’re good to go. It works for me every time on FreeBSD, so it should work for you too.

## When to Use It 🕒

Here's the kicker: **you don’t need to run this every time**. Just run it **once** after you've created your new project (whether it's `ng new` for Angular, `npx create-react-app` for React, or whatever you're using). Let this script handle the messy parts so you can focus on building cool stuff.

1. Create your project like normal:
   ```bash
   ng new my-cool-project
   # or
   npx create-react-app my-app
   ```

2. Then hit it with:
   ```bash
   ./freebsd-rollup.sh
   ```

3. And just like that, *boom*, you're back to slinging code.

## Installation & Usage 💻

1. Clone this repo or download the script:
   ```bash
   git clone https://github.com/yourusername/freebsd-rollup.git
   ```

2. Navigate to the project folder and run the script:
   ```bash
   cd freebsd-rollup-fix
   chmod +x freebsd-rollup.sh
   ./freebsd-rollup.sh
   ```

## What It Does Behind the Scenes 🕵️‍♂️

- **Installs** the `@rollup/wasm-node` package, making Rollup **FreeBSD-friendly**.
- **Replaces** the Rollup native configuration with a custom patch to let it run smoothly on your FreeBSD setup.
- Keeps your build process clean and avoids those nasty `npm` dependency errors!

## Why @rollup/wasm-node? 🧙‍♂️

We're using **WASM** (WebAssembly) for a reason, my friend! Since FreeBSD doesn’t play nice with all those native builds, **wasm-node** lets us sidestep the issue. It’s lightweight, fast, and it won’t break your dev flow.

## License 📝

**MIT** – Feel free to use, remix, and share. If this helps you, shout me out or give the repo a star ⭐!

