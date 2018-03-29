## Detail opportunity with GSA

We're looking for a detailee to GSA's Technology Transformation Services (TTS), in the Office of Products and Programs (OPP), who can drive [this project](project.md) forward in a full-time capacity.

### What the detailee would do

The detailee would own the development and technical direction of an **infrastructure project** to better discover, collect, and analyze information about the federal government's substantial online surface area of internet-facing services.

Read [this project description](project.md) for a full description.

The work will include:

* Identifying useful technical information to collect about internet-facing federal services, and implementing software to collect this information.
* Identifying new data sources for discovering what internet-facing services the federal government operates, and implementing support for these sources.
* Identifying ways to improve the speed and scale of the underying infrastructure, and implementing these technical improvements.
* Deepening our partnerships with the Department of Homeland Security, the White House Office of Management and Budget, and other federal agencies, in support of government-wide initiatives and the dissemination of actionable data to the federal enterpirse.
* Supporting open source reuse of this infrastructure with other organizations.

### Requirements

From a technical perspective, the detailee should:

* Have significant experience with software engineering, particularly in developing "backend" systems and the use of command line tools. Experience with "frontend" and web development is also very helpful.
* Be very comfortable writing Python code. Proficiency with JavaScript is also very helpful.
* Have significant experience with internet protocols and concepts. Expertise with every major apect of the internet is definitely _not_ required. However, protocols such as HTTP and DNS should be reasonably well-understood, and the detailee should be able to quickly learn about new protocols as they become relevant.
* Have significant experience with web platform concepts. Expertise with every web platform feature is definitely _not_ required. However, concepts such as CSS, cookies, and referrer headers should be reasonably well-understood. The detailee should be familiar with browser development tools and comfortable using them to understand the mechanics of web services.


## Where the project could go

There are many possibilities of where to take this project. The priorities and roadmap are not decided.

Below are some ideas, but these are just some options. The detailee will help determine the priorities of the project, and where to invest effort for maximum return to GSA and to the federal government.

#### Expanding what things we look at

* Identifying the use of third party services (such as analytics/behavior trackers, content CDNs, or accessibility tools) and their privacy and security impacts on users of government services.
* Mobile friendliness, particularly in response to recent federal requirements around making new websites mobile friendly.
* Identifying missing, misconfigured, or outdated integrations of the [Digital Analytics Program](https://analytics.usa.gov).
* Lightweight crawling and archiving of federal web services, in ways that may support search use cases like Search.gov, or archiving use cases like those the Library of Congress performs.
* Whatever becomes interesting next! Part of the point of this work is to be able to drastically shorten the feedback loop between federal staff having a new question, and having the answer to that question.

#### Improving how we look at things

* Analyzing more than just domain names. Right now, the service is oriented around domain names, and website analysis is typically performed only at the homepage. Expanding this to accommodate multiple URLs within a domain name would be a prerequisite to certain kinds of crawling and analysis.
* Including more than just `.gov` and `.fed.us` hostnames. Though most services use `.gov`, `.fed.us`, and `.mil`, the federal government does still make extensive use of other suffixes, especially for partnerships with the private and non-profit sectors. GSA has [attempted to collect some of this data before](https://github.com/GSA/govt-urls), but the effort has been inactive for the last few years.
* Examining alternate cloud-based pipelines to Amazon Lambda, such as Google Cloud Functions or Amazon Batch, which may offer different properties that make them more well suited for certain kinds of tasks.
* Self-service scanning for federal government staff. For example, we could provide simple scanner templates (or a hosted web service) that allow staff in other agencies to write small amounts of simple measurement code, and then run that code inside of our infrastructure. Agencies would automatically receive data within hours or minutes. Submissions could be subject to review by GSA staff, or we could allow trusted non-GSA federal staff to run scans without waiting for our involvement.
* Integrating non-public datasets. Right now, we limit ourselves to analyzing services that are already publicly discoverable, but this does leave a gap. We could partner with federal programs (such as DotGov or DotMil), or create paid arrangements with commercial partners, to grow our understanding of the federal government's surface area.
