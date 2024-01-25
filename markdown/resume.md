David Holt
============

Software Developer
-----------------

* Full stack software developer with many years' experience designing and building multi-tiered applications, both in traditional data centers and in the cloud.

* Knowledge of commercial and open-source softwarek/database engineering tools and design techniques.

* Multiple years' experience working on agile teams.

Education
---------

1998-1999
:   **AAS in Computer Programming**; Minneapolis Community and Technical College (Minneapolis, MN)

Experience
----------

### Chewy, Inc. - Boston, MA

**Software Entineer II**, 2021-2022

Work on agile teams to design, develop and maintain software to support managers in Chewy's fulfillment centers.

* Labor Planning

    * I had a small part of the migration of our Labor Planning application to AWS. Primarily, I designed and implemented the integration testing framework for the application. I utilized [Testcontainers](https://testcontainers.com) running PostgreSQL for data access and [LocalStack](https://www.localstack.cloud) for the AWS calls, which allowed us to test the full stack without the need for a network connection beyond the local machine. This gave us dependably repeatable integration tests.

* Performance Management

    * Helped to design and implement the revamped Performance Management application. This system tracks performance metrics such as *attendance*, *productivity* and *quality*, and generates scorecards for each team member. Area managers can then use the scorecards to identify team members who need more training, or are consistently below the expected standards of performance. This system replaced a manual process involving an Access DB and Excel spreadsheets.

    * Wrote the SQL scripts for the for the attendance metrics, which pulled data from the Data Warehouse and aggregated it for the scorecards.

    * Brought in the testing framework I developed for Labor Planning into Performance Management project.

* Chewy Labor Management System (CLMS) migration to AWS

    * CLMS was a job scheduler and runner for a variety of different tasks, such ingestion of:

        * punch data from Kronos

        * labor log data from the Körber WMS system

    Many of the jobs ran for each of the 10+ fulfillment centers sequentially.

    * I designed and implemented a new version of CLMS to run in AWS. The new system makes multiple improvements to the current design:

        * The scheduler and runner component are now separate modules, so each could be modified and scaled independently.

        * Tasks can be scheduled or run in response to events.

        * Tasks can be run in parallel allowing scorecards to be generated much faster. One benefit of this is allowing scorecards to be updated in realtime, allowing more frequent feedback for managers and team members.

    * The new solution made use of the following technologies:

        * AWS EventBridge

        * AWS SQS

        * AWS Lambda

        * AWS Fargate

        * AWS RDS/Aurora PostgreSQL

        * Java/Spring Boot for Lambdas

        * JavaScript/VueJS for front-end

### Cox Automotive, Inc. - Dallas, TX

**Software Entineer II**, 2015-2019

Worked on agile teams to design, develop and maintain inventory data intake and display solutions for various Cox Automotive business units, using Java and related tools.

* Converted existing Jenkins build environment for Vehicle Consumer Display API (VCDA) to AWS Code Build/Code Pipeline using Terraform and Terragrunt to deploy the infrastructure.

* Converted VCDA public endpoints from Mashery to AWS API Gateway, using Terraform.

* Helped design and develop VCDA in the AWS cloud using Java microservices. This solution consisted of a producer in the data center that responded to inventory change events and captured the vehicle record and pumped it into Kinesis Firehose, which ultimately stored the record in AWS S3 for further processing; a consumer service in AWS that processed the vehicle record, converting it to the format supported by VCDA, enriching it in various ways (such as adding price and incentives information), and breaking the monolithic record from the data center into smaller documents that could be retrieved as needed—the main vehicle document was stored in Elasticsearch to support indexed searching, while supplementary documents (price, lease/loan payments, incentives, etc.) were stored in DynamoDB; and a series of microservices which exposed APIs for searching vehicles and returning the various parts as needed. The AWS services were deployed and auto scaled by Elastic Beanstalk. These services were implemented as Spring Boot applications.

* Helped design and develop intake process to feed data from our legacy inventory system into the AWS cloud to feed VCDA, using Java.

* Helped design and develop the AWS infrastructure-as-code using Terraform

### DealerTrack Technologies - Dallas, TX

**Software Entineer**, 2012-2015

Worked on agile teams maintaining and enhancing the ClickMotive Fusion web platform for automobile dealer websites. DealerTrack Technologies acquired ClickMotive competitor Dealer.com in 2013 and decided to focus on the Dealer.com platform. At that time, I transitioned onto Dealer.com team, and began to support that platform, developing and maintaining inventory data intake and display Dealer.com business unit. *DealerTrack was acquired by Cox Automotive in Oct 2015*.

* Developed UI for displaying Google Analytics data using NVD3.js and D3.js.

* Developed test suite for Analytics reporting functionality using Jasmine.js.

* Maintained and enhanced Inventory intake application.

* Maintained and enhanced Inventory Services application, which aggregated data from multiple sources to provide a unified view of a Vehicle for consumption by Dealer websites, analytics and syndication.

* Maintained and enhanced Content Syndication application, which syndicated inventory data in various custom formats, as dictated by consumers.

### ClickMotive - Plano, TX

**Applications Developer**, 2008-2012

Worked on agile teams maintaining and enhancing the ClickMotive Fusion web platform for automobile dealer websites. *ClickMotive was acquired by DealerTrack Technologies in Oct 2012*.

* Designed and developed C# replacement for Google AdWords generator that had been implemented in SQL Server using cross joins. Used RavenDB NoSQL Database for data store.

* Designed and developed various "skins" for Fusion platform; these were custom HTML/CSS/JavaScript addons to the platform to provide customer specific customizations. Used jQuery JavaScript library and SASS/SCSS for styling.

### Verizon Corporation - Irving, TX

**Developer Contractor**, 2006-2008

Provided independent IT services (separate from Verizon ID department) for a small team that designed, implemented and tracked results from advertising campaigns.

* Maintained the existing Campaign Manager, written in VB.NET, with a MySQL database.

* Designed and developed the replacement Campaign Manager. Technologies used included C#, SQL Server, JavaScript, HTML and CSS.

### HighJump Software - Eden Prairie, MN

**Product Development Engineer**, 1999-2005

Worked in a traditional waterfall environment, designing and developing supply chain execution software.

* Designed, developed and maintained an onscreen keyboard in Visual Basic intended for touch screen kiosks in the warehouse.

* Designed, developed and maintained a simple application in Visual Basic to allow a PC with a barcode scanner attached function as a Data Collection Device.

* Converted the dialogs for our in-house development tool from C to C++ and refactored them to abstract out common functionality.

* Worked on the defect team, diagnosing and fixing defects in the full range of our applications. From our Engine (a special purpose OS designed for supply chain execution applications), to our Development Tool, to WebWise our web tool for creating web-based supply chain applications. Technologies used included C/C++, Visual Basic, SQL Server, Oracle, CodeBase (a C library for working with DBF file, now opened sourced as [CodeBase-for-DBF](https://github.com/MPSystemsServices/CodeBase-for-DBF)), and Visual FoxPro (used for querying our DBF files).

Technical Summary
-----------------

AWS, Bash, Bootstrap, C, C++, C#, CSS/SCSS/Sass, Elixir, Gradle, Handlebars, HTML, Jasmine, Java, JavaScript, Jenkins, JQuery, Lodash, Maven, Mocha, MongoDB, MySQL, .NET, NodeJS, Phoenix, PostgreSQL, Python, Rails, RavenDB, Redis, Ruby, Spring, SQL, SQL Server, TeamCity, Terraform, XML


> <dpjh747@example.com> • +1 (216) 318-0103 • 57 years old\
> 3613 Lynnfield Rd Apt 1, Shaker Heights, OH, USA
