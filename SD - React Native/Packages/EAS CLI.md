**Install EAS CLI**
```sh
npm install --global eas-cli
```

**Log in to EAS**
```sh
eas login
```

**Configure EAS Build**
```sh
eas build:configure
```

**Build Android Development APK**
For development or testing
```sh
eas build --platform android --profile development
```

**Build Android Preview APK**
Testing a production-like app
```sh
eas build --platform android --profile preview
```

**Build Android Production APK**
Actual release
```sh
eas build --platform android --profile production
```

**EAS JSON Setup**
```
{
  "cli": {
    "version": ">= 21.8.0",
    "appVersionSource": "remote"
  },

  "build": {
    "development": {
      "developmentClient": true,
      "distribution": "internal",
      "env": {
        "APP_VARIANT": "development"
      }
    },

    "preview": {
      "distribution": "internal"
    },

    "production": {
      "autoIncrement": true,
      "android": {
        "buildType": "apk"
      }
    }
  },

  "submit": {
    "production": {}
  }
}
```

**Separate APKs for Production and Development**
Rename `app.json` to `app.config.ts`
```ts
import type { ExpoConfig } from "expo/config";

const config: ExpoConfig = {
  name: "mobile",
  slug: "mobile",
  version: "1.0.0",
  orientation: "portrait",

  icon: "./assets/images/icon.png",

  scheme: "mobile",

  userInterfaceStyle: "automatic",

  ios: {
    icon: "./assets/expo.icon",
  },

  android: {
    package: "com.jpamada.mobile",

    adaptiveIcon: {
      backgroundColor: "#E6F4FE",
      foregroundImage: "./assets/images/android-icon-foreground.png",
      backgroundImage: "./assets/images/android-icon-background.png",
      monochromeImage: "./assets/images/android-icon-monochrome.png",
    },

    predictiveBackGestureEnabled: false,
  },

  web: {
    output: "static",
    favicon: "./assets/images/favicon.png",
    bundler: "metro",
  },

  plugins: [
    "expo-router",

    [
      "expo-splash-screen",
      {
        backgroundColor: "#208AEF",
        image: "./assets/images/splash-icon.png",
        imageWidth: 76,
      },
    ],

    "expo-sqlite",
    "expo-image",
    "expo-sharing",
  ],

  experiments: {
    typedRoutes: true,
    reactCompiler: true,
  },

  extra: {
    router: {},
    eas: {
      projectId: "d30106cc-4128-43f8-bdeb-a80bcebe3052",
    },
  },
};

if (process.env.APP_VARIANT === "development") {
  config.name = "Mobile Dev";

  config.android = {
    ...config.android,
    package: "com.jpamada.mobile.dev",
  };

  config.ios = {
    ...config.ios,
    bundleIdentifier: "com.jpamada.mobile.dev",
  };
}

export default config;
```

**Change EAS Project ID**
```json
extra: {
  router: {},
  eas: {
    projectId: "666fb853-07d5-413b-b636-e64ceb46b31b",
  },
},
```