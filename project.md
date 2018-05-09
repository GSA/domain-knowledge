## Discovering and improving the federal government's online services

This project has three major components:

* **Discovering the federal government's online services**, and sharing this information with our federal partners and the entire federal community.

* **Collecting information about these services** that can be used to accelerate the modernization of the federal government's technology offerings and security posture.

* **Building and scaling the infrastructure that enables these efforts**, using modern cloud-based tools to perform rapid, internet-scale data analysis.

### Current work

GSA has already done significant work on systems for discovering and analyzing the federal government's online services.

This work has also been part of a close open source collaboration with the Department of Homeland Security's Cyber Hygiene team. The project also sees contributions from NASA, Lawrence Livermore National Laboratory, and other  organizations from around the world.

* We discover as many publicly accessible.gov web services as we can, [using publicly discoverable data](https://pulse.cio.gov/https/guidance/#subdomains) from government and private-sector sources. This data is used as part of [Pulse](https://pulse.cio.gov), the [Department of Homeland Security's Cyber Hygiene reporting](https://18f.gsa.gov/2017/01/06/open-source-collaboration-across-agencies-to-improve-https-deployment/), and other government projects.

* This work is currently oriented around feeding government-wide reporting on web and email security, in support of initiatives like [OMB's HTTPS-only policy](https://https.cio.gov), and [DHS' web and email security directive](https://cyber.dhs.gov/bod/18-01/).

### Technical components

The core technical project that is [`domain-scan`](https://github.com/18f/domain-scan), which provides two core functions:

1. Discovering hostnames from various sources, filtering them based on given parameters (such as being within a certain suffix or set of base domains), and generally dedupes/cleans/synthesizes that data into a final report. Includes specialized support for [Censys.io](https://censys.io).

2. Orchestrating overall scanning processes, using a mix of local and cloud-based parallelization. Used to instrument open source tools like DHS' [`pshtt`](https://github.com/dhs-ncats/pshtt) and [`trustymail`](https://github.com/dhs-ncats/trustymail), as well as [SSLyze](https://github.com/nabla-c0d3/sslyze) and other tools. Includes specialized support for [Amazon Lambda](https://aws.amazon.com/lambda/), headless Chrome, and [Puppeteer](https://github.com/GoogleChrome/puppeteer).

It's likely that [`domain-scan`](https://github.com/18f/domain-scan) will be split into two separate tools, but for now they are combined into one repository.

