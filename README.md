https://guykawasaki.com/the-only-10-slides-you-need-in-your-pitch/

## Run a development environment

The development environment will connect to the cbase.codefor.nl BASE_URI by default. Override it if you have a local setup for the API too.

```
docker build -t pitchdeck_dev_local:0.0.1 .
docker run -v $(pwd)/public:/var/www/html/public -v $(pwd)/private:/var/www/html/private -p 8080:80 pitchdeck_dev_local:0.0.1
```

You can then access the site at http://localhost:8080 and make changes in your local php files.
