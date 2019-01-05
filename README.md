# Simple Docker Container for Wkhtmltopdf

Uses Centos 7 package from the official site, running Amazon Linux (latest).

## Usage

wkhtmltopdf with qt patches - latest version as of 5 Jan 2019

```
# build yourself
docker build -t docker-wkhtmltopdf .
docker run docker-wkhtmltopdf google.com - > test.pdf

# from URL
docker run docker-wkhtmltopdf google.com - > test.pdf

# from mounted local file (e.g. test.html)
docker run --rm -v $(pwd):/data docker-wkhtmltopdf /data/test.html - > test.pdf
```




