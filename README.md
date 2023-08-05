# todo-list

Todo List App with React Native.

## Installations

> Install all dependency packages.

```bash
npm install
```

> Please install the expo application on your smartphone to debug.

## Running

> Run with command

```bash
npm run start
```

## Production

> With EAS build

```bash
# login your eas account
eas login

# make sure your account has been login
eas whoami

# generate build configure
eas build:configure
```

> Modify `eas.json` like this

```json
{
  "build": {
    "preview": {
      "android": {
        "buildType": "apk"
      }
    },
    "preview2": {
      "android": {
        "gradleCommand": ":app:assembleRelease"
      }
    },
    "preview3": {
      "developmentClient": true
    },
    "production": {}
  }
}
```

> Start your build with the following command

```bash
eas build -p android --profile preview
```

## License

This project is under the MIT License.
