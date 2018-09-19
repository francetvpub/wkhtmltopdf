# wkhtmltopdf Docker image

Containerized `wkhtmltopdf` and `wkhtmltoimage` on debian:jessie base.

- For Docker image: [etelej/wkhtmltopdf](https://hub.docker.com/r/etelej/wkhtmltopdf/)



# Basic Usage

Generate PDF from website/url
```
docker run --rm -v "$PWD":/cwd etelej/wkhtmltopdf wkhtmltopdf https://quotes.etelej.com /cwd/out.pdf
# generates out.pdf current directory
```

Generate PDF from HTML file (e.g. page.html in current directory)
```
docker run --rm -v "$PWD":/cwd etelej/wkhtmltopdf wkhtmltopdf cwd/page.html /cwd/out.pdf
# generates out.pdf at current directory
```


