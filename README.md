# Seam docs

### Set up

Install the [Github desktop app](https://desktop.github.com/). This will enable you to push the changes you make locally to the Github repo. Any changes pushed to the repo will be picked up by the Mintlify Github app and published to the site.

<img width="1514" alt="Screenshot 2024-04-15 at 10 10 46 AM" src="https://github.com/signal-data/signal-docs/assets/13254616/55c81dc8-4ecd-45de-b53e-b83d351bc858">

Go back to the [repo page on Github](https://github.com/signal-data/signal-docs) and clone the repository to your local environment.

<img width="2372" alt="Screenshot 2024-04-15 at 10 13 22 AM" src="https://github.com/signal-data/signal-docs/assets/13254616/d293e06d-6e4f-430e-b1be-37f7f692af1f">

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify). This only needs to be done once. To install, use the following command:

```
npm i -g mintlify
```

### Development

Run the following command at the root of your documentation (where mint.json is) to preview the documentation changes locally in the browser at `http://localhost:3000`. When any changes are made and saved, the preview will rerender immediately to show the changes.

```
mintlify dev
```

<img width="2372" alt="Screenshot 2024-04-15 at 10 14 31 AM" src="https://github.com/signal-data/signal-docs/assets/13254616/1fe71cb8-60b6-4980-9619-38963b06d79a">

### Publishing Changes

When you are ready to publish your changes, use the Github desktop app to commit and push the changes you have made. Changes will be deployed to production automatically after pushing to the `main` branch. 

### Troubleshooting

- Mintlify dev isn't running - Run `mintlify install` it'll re-install dependencies.
- Page loads as a 404 - Make sure you are running in a folder with `mint.json`
