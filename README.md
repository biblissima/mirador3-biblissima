
# mirador3-biblissima

This repository is for the [Mirador 3](https://github.com/ProjectMirador/mirador/) instance used by the [Biblissima portal](https://portail.biblissima.fr).

The Biblissima instance includes several customizations to adjust initialization settings and a few plugins to extend viewer's functionality.


## Install dependencies:

```
npm install
```

## Start app

Open `demo/index.html` on localhost:4444 and watch the source files:
```
npm start
```

URL: http://localhost:4444/?iiif-content=https://gallica.bnf.fr/iiif/ark:/12148/btv1b525002505/manifest.json

Existing URL parameters are:

- `iiif-content`: URL of IIIF resource (Manifest or Collection) or encoded IIIF Content State
- `mode`: mirador embedding mode (depending on the host page in the Biblissima portal). Possible values are:
    - `single`: load a single IIIF resource, without workspace
    - `catalog`: bypass the collection modal and populate the catalog window directly with all the child manifests
- `panel`: select which side panel to open when the viewer is initialized (only `info` is supported)
- `theme` = mirador selected theme

## Serve demo

Serve static files in `demo/portal` on localhost:5555
```
npm run serve
```

Directory root: http://localhost:5555/demo/portal
