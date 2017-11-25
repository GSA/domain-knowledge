
Working syntax for doing a full gather of publicly discoverable federal .gov subdomains:

> ./gather censys,dap,eot2016,rdns-snapshot,parents --eot2016=https://github.com/GSA/data/raw/master/end-of-term-archive-csv/eot-2016-seeds.csv --rdns-snapshot=https://github.com/GSA/data/raw/master/dotgov-websites/rdns-federal-snapshot.csv --dap=https://analytics.usa.gov/data/live/sites-extended.csv --suffix=.gov,.fed.us --parents=https://github.com/GSA/data/raw/master/dotgov-domains/current-federal.csv --include-parents --ignore-www --debug --export --force

If you can't access Censys.io Export APIs and need to rely solely on remote CSVs:

> > ./gather censys-snapshot,dap,eot2016,rdns-snapshot,parents --censys-snapshot=https://github.com/GSA/data/raw/master/dotgov-websites/censys-federal-snapshot.csv --eot2016=https://github.com/GSA/data/raw/master/end-of-term-archive-csv/eot-2016-seeds.csv --rdns-snapshot=https://github.com/GSA/data/raw/master/dotgov-websites/rdns-federal-snapshot.csv --dap=https://analytics.usa.gov/data/live/sites-extended.csv --suffix=.gov,.fed.us --parents=https://github.com/GSA/data/raw/master/dotgov-domains/current-federal.csv --include-parents --ignore-www --debug --force

TODO:

* Update to latest EOT 2016 data (they have more stuff up til May)
* Look at our own crawling infrastructure
