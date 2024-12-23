# Web - lang and dir attributes not respected

The `app.json` documentation specifies that [dir](https://docs.expo.dev/versions/latest/config/app/#dir) and [lang](https://docs.expo.dev/versions/latest/config/app/#lang) attributes can be set for the `web` but this does not work both in development server neither in the exported web build.


## Steps to reproduce



```bash
npx create-expo-app@latest StickerSmash
cd StickerSmash
npm run web
```

And now the `lang` and `dir` attribute won't be set even though they are set already in `app.json`

While exporting:

```bash
npx expo export
npx expo server
```

And the generated output also would not have the `lang` and `dir` attributes set.
