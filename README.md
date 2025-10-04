# Welcome to your Expo app 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
   npx expo start
   ```

In the output, you'll find options to open the app in a

- [development build](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go), a limited sandbox for trying out app development with Expo

You can start developing by editing the files inside the **app** directory. This project uses [file-based routing](https://docs.expo.dev/router/introduction).

## Team setup (Windows / PowerShell)

If you're collaborating and want a consistent environment on Windows (PowerShell), follow these steps:

1. Install Node.js matching the project's recommended version. We use Node 20.19.4. If you use nvm for Windows, you can run:

```powershell
nvm install 20.19.4
nvm use 20.19.4
```

Alternatively, follow the installer at https://nodejs.org.

2. Install project dependencies:

```powershell
cd <project-root>
npm install
```

3. Start the Expo dev server (PowerShell):

```powershell
npm run start
```

4. Common issues and fixes

- If you see warnings about Node engine versions during `npm install`, use the Node version in `.nvmrc` to match the environment.
- If Metro fails to start or you see stale caches, run:

```powershell
npx expo start -c
```

### If you see a legacy Expo CLI / ExpoMetroConfig error

If your terminal shows a message like:

```
WARNING: The legacy expo-cli does not support Node +17. Migrate to the new local Expo CLI
ExpoMetroConfig.loadAsync is not a function
TypeError: ExpoMetroConfig.loadAsync is not a function
```

This usually means a globally-installed (deprecated) `expo-cli` is being used instead of the local Expo CLI bundled with the `expo` package.

Fix steps (PowerShell):

```powershell
# 1) Uninstall the global legacy CLI (if installed)
npm uninstall -g expo-cli

# 2) Use the local CLI with npx (recommended)
npx expo start

# Or use the npm script we added which runs the local CLI:
npm run start:local
```

Removing the global `expo-cli` ensures the project uses the newer, supported local CLI and resolves `ExpoMetroConfig.loadAsync` errors.

- If your coworkers use macOS or Linux, these instructions still apply; use their platform's package manager or nvm implementation.

## Additional scripts

We provided a convenience script `npm run reset-project` that will move starter code to `app-example` and create a blank `app` directory if you need a clean slate for demos or starter work.

## Get a fresh project

When you're ready, run:

```bash
npm run reset-project
```

This command will move the starter code to the **app-example** directory and create a blank **app** directory where you can start developing.

## Learn more

To learn more about developing your project with Expo, look at the following resources:

- [Expo documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with our [guides](https://docs.expo.dev/guides).
- [Learn Expo tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial where you'll create a project that runs on Android, iOS, and the web.

## Join the community

Join our community of developers creating universal apps.

- [Expo on GitHub](https://github.com/expo/expo): View our open source platform and contribute.
- [Discord community](https://chat.expo.dev): Chat with Expo users and ask questions.
