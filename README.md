# Seam docs

## Set up

Install the [Github desktop app](https://desktop.github.com/).

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify). This only needs to be done once. To install, use the following command:

```
npm i -g mintlify
```

## Development

Run the following command at the root of your documentation (where mint.json is) to preview the documentation changes locally in the browser at `http://localhost:3000`. When any changes are made and saved, the preview will rerender immediately to show the changes.

```
mintlify dev
```

To stop

## Publishing Changes

Install our Github App to autopropagate changes from youre repo to your deployment. Changes will be deployed to production automatically after pushing to the default branch. Find the link to install on your dashboard.

#### Troubleshooting

- Mintlify dev isn't running - Run `mintlify install` it'll re-install dependencies.
- Page loads as a 404 - Make sure you are running in a folder with `mint.json`
