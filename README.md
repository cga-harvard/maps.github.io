# maps.github.io
## Repository for redirects for maps.cga.harvard.edu
### General Instructions
[https://docs.github.com/en/pages/quickstart](https://docs.github.com/en/pages/quickstart)

### Redirecting maps.cga.harvard.edu and maps.cga.harvard.edu/tgaz:
1.  Create a repository named maps.github.io  The repository name must end in github.io

1.  Create a file called `CNAME` with the contents
```
maps.cga.harvard.edu
```

3.  Set your DNS CNAME in the HUIT DNS for `maps.cga.harvard.edu` to point to `cga-harvard.github.io`  This has to be done before step 5.

1.  Place this file in the top level directory:
```
<!DOCTYPE html>
<html>
  <head>
    <meta http-equiv="refresh" content="0; url=https://gis.harvard.edu/" />
    <title>Redirecting…</title>
    <link rel="canonical" href="https://gis.harvard.edu/" />
  </head>
  <body>
    <p>If you are not redirected, <a href="https://gis.harvard.edu/">click here</a>.</p>
  </body>
</html>
```

5.  Go to your repo’s `Settings > Pages`.  Under “Custom domain”, enter `maps.cga.harvard.edu` and save.

1.  Enable `Enforce HTTPS` once the custom domain is recognized.

1.  Create a directory called `tgaz`

1.  Place this file in the tgaz directory:
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
