# maps
## Repository for redirects for maps.cga.harvard.edu
General directions can be found here:
[https://docs.github.com/en/pages/quickstart](https://docs.github.com/en/pages/quickstart)

This is specific to this repository:
1.  Create a repository named maps.github.io  The repository name must end in github.io

1.  Create a file called `CNAME` with the contents
```
maps.cga.harvard.edu
```

1.  Set your DNS CNAME in the HUIT DNS for `maps.cga.harvard.edu` to point to `cga-harvard.github.io.`  This has to be done before step 3.

1.  Go to your repo’s `Settings > Pages`.  Under “Custom domain”, enter `maps.cga.harvard.edu` and save.

1.  Enable `Enforce HTTPS` once the custom domain is recognized.

1.  Create a directory called `tgaz`

1.  Place this file in the directory:
```
<!DOCTYPE html>
<html>
  <head>
    <meta http-equiv="refresh" content="0; url=https://chgis.hudci.org/" />
    <title>Redirecting…</title>
    <link rel="canonical" href="https://chgis.hudci.org/" />
  </head>
  <body>
    <p>If you are not redirected, <a href="https://chgis.hudci.org/">click here</a>.</p>
  </body>
</html>
```
