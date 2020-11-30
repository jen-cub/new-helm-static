# Static Site Helm Chart

---

## Updating repository with new chart version

```
make
```

The simple command `make` will:
-   Create a directory (../planet4-helm-charts by default) to store chart bucket contents
-   Pull contents of P4 Helm GCS bucket
-   Package the current directory as a new chart version
-   Move the packaged chart to the local chart directory
-   Update the index
-   Synchronise local chart directory with GCS bucket contents

For managing repository updates it is strongly recommended to use https://github.com/viglesiasce/helm-gcs
