# Disney Plus API
Get episode titles and release dates of Disney+ series

### Want to contribute?
- Create a PR

### Adding a new title
Use a web browser that support Disney+

Get the short link of the Disney+ series

e.g. moon-knight

![](Screenshot%202022-05-31%20232403.png)

Open Developer tools and observe the Network tab for Fetch/XHR requests

Look out for a request URI `DmcSeriesBundle` and note the URI down

e.g. https://disney.content.edge.bamgrid.com/svc/content/DmcSeriesBundle/version/5.1/region/SG/audience/k-false,l-true/maturity/1870/language/en-GB/encodedSeriesId/4S3oOF1knocS

![](Screenshot%202022-05-31%20233339.png)

Take the short link and the URI and present it in a key:value format
```json
"moon-knight": "https://disney.content.edge.bamgrid.com/svc/content/DmcSeriesBundle/version/5.1/region/SG/audience/k-false,l-true/maturity/1870/language/en-GB/encodedSeriesId/4S3oOF1knocS"
```

Update series.json and create a pull request
