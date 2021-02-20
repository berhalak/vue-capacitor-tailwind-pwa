
## Setup

Use npm as yarn has some problems with capacitor comunity electron


```
yarn create @vitejs/app vue-capacitor-tailwind-pwa --template vue
cd vue-capacitor-tailwind-pwa
yarn 
yarn build
yarn add -D @capacitor/core @capacitor/cli
npx cap init test test.antyprojekt.pl --web-dir=dist
```

## Build android
setup

```
npx cap add android
```

run

```
npx cap copy
# requires android studio
npx cap open android
```


## Build electron

Setup

```
yarn add -D @capacitor-community/electron
npx cap add @capacitor-community/electron

```

Run

```
npx cap copy
npx cap open @capacitor-community/electron
```

## Build web


```
npx cap copy
npx cap serve
```

## Add pwa to vite

```

npm i vite-plugin-pwa -D

```