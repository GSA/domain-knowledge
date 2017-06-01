
Working syntax for doing a full gather of publicly discoverable federal .gov subdomains:

> ./gather censys,dap,eot2016,parents --eot2016=https://github.com/GSA/data/raw/gh-pages/end-of-term-archive-csv/eot-2016-seeds.csv --dap=https://analytics.usa.gov/data/live/sites-extended.csv --suffix=.gov --parents=https://raw.githubusercontent.com/GSA/data/gh-pages/dotgov-domains/current-federal.csv --include-parents --debug --export --force

TODO:

* Update to latest EOT 2016 data (they have more stuff up til May)
* Look at our own crawling infrastructure
