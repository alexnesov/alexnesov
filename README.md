### Hi there 

I'm Alex Nesovic. Worked first in technology consulting at Accenture Technology, then worked for the Capital Markets division of Deloitte Luxemboug (Alternative Investments sub-division) as a Senior Consultant (Software Developer using Python, Flask, JS). Worked also for one fund manager's technology division as a tech consultant for the front-office and middle-office side of their client's operations. <br>

# Technical Portfolio

  
## Financial-portfolio.io (new version)

[![financial-portfolio.io](https://github.com/alexnesov/alexnesov/blob/main/vanillaJS/Assets/fp_logo.svg)](https://www.youtube.com/watch?v=HUfxmiZ7kGs)
  
**[Click here to see demo of parallelization integrated into financial-portfolio.io](https://www.youtube.com/watch?v=HUfxmiZ7kGs)**


Please switch to 1440p and above to be able to see the logs.

Tech stack: React, Redux, Django, Docker, Celery, Redis
Protocols: WebSocket (ensures real-time component updates and avoids waiting for the entire page to load) & HTTPS
In Production: AWS Beanstalk is provisioned to ensure scalability, thanks to it's auto-scaling capability.

All 4 financial research processes (can scale way up of course) were launched exactly at the same time by a JS command here locally and where handled in parallel (see "About the logs" in the description below).

As you can see, the financial data was fetched almost at the same time. "Almost" because this data was retrieved on a different time depending on where it was located in my DBs.
The Financial News data can't appear strictly at the same time for the 4 different tickers because the retrieval time itself varies depending on the complexity of the research that has to be conducted on the Web. 

**About the logs:** <br>
They demonstrate that my application leverages parallelization using Celery's prefork pool, with multiple worker processes (ForkPoolWorker-X) running tasks concurrently, optimizing performance by executing tasks in parallel across different CPU cores.

Contact: https://www.info-com.io/



## Financial-portfolio.io (old version)

"Official" version is currently off the grid but demo available here: http://financial-portfolio.eu-central-1.elasticbeanstalk.com/  (not optimized for mobile)

This project gives an overview of my capabilities (full-stack, from server setup on the back end, though front-end design, to cloud deployment with Docker and routing for public availability).

<b>Financial-portfolio.io (AWS cloud-native) is: </b>
1. An autonomous market data feeder powered by Python, Jenkins/Cron and Linux. A stock market data platform accessible via a own developed front-end.
2. An autonomous signals detector

<b>Development performed on FP : </b>

<b>Second Phase:</b> <br> (**!! The code of the commercial and extended version is private, let's get in touch if you'd like to know more !!**)
- Currently migrating the project from Flask/JS (+AJAX, Jquery) to a Django/React tech stack
- Setting up Redux to manage the global state

<b>First Phase:</b> <br>
- Deployed the app (Python Flask application) to the web & the cloud (AWS Route 53, Beanstalk & Docker)
- Implemented the automated & scheduled web crawlers to scan the American stock market on a daily basis (Python Selenium + Jenkins on Linux AWS EC2 VMs)
- Coded the automated technical analysis algorithms (Python)
- Coded the front-end (JS, HTML, CSS, Bootstrap)
- Coded the middleware (AJAX calls <-> Flask API)
- User authentication procedure developement
- AWS RDS MySQL setup 
- Connection to different market data API's

Code (first phase): https://github.com/alexnesov/Financial-portfolio-Flask

<img src="https://github.com/alexnesov/Financial-portfolio-io-advanced-Flask/blob/main/SV/static/signal_flow_na2.png">
<img src="https://github.com/alexnesov/Get-the-signals/blob/8dab1ac794c2fe0524169f6ca1cd316cad621bf1/SV/static/dash.png">

## Project-based.io

### Architecture of the app

<img src="https://github.com/alexnesov/project_based_io/blob/main/documentation/diagrams/data_flow.png">


# My Skills

## Languages
- <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/> (my strong point, using it daily in a professional (Accenture, Deloitte, Axa, Clearstream) and personnal context, since 4 years almost)
- <img alt="JS" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/> 
- <img alt="cpp" src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white"/> (basics)
- <img alt="java" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white"/> (basics)
- <img alt="C" src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white"/> (basics)


## DB's
- <img alt="sqlite" src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white"/>
- <img alt="mysql" src="https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white"/>

## Web

### Servers & API's
- <img alt="flask" src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white"/> (using it daily)
- <img alt="Django" src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=green"/>
- <img alt="Django-REST" src="https://img.shields.io/badge/DJANGO-REST-ff1709?style=for-the-badge&logo=django&logoColor=white&color=ff1709&labelColor=gray"/>
- Using Postman and exporting the JSON format configs for API documentation. Used Swagger also a bit.

### Front-end & Middleware
- <img alt="HTML" src="https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=white"/>
- <img alt="CSS" src="https://img.shields.io/badge/CSS-239120?&style=for-the-badge&logo=css3&logoColor=white"/> (hands-on native CSS flexbox usage, after having sweat with float handling)
- <img alt="Bootstrap" src="https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white"/>
- <img alt="react" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB"/> 
- <img alt="redux" src="https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white"/> 
- Used AJAX with vanilla JS before, JQuery also, but currently using REST arch with JSON, daily, in the context of React developments
- Learning ThreeJS
- Using Electron for Desktop development 

## Cloud

   
- <img alt="aws" src="https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white"/>
- Daily usage of EC2 (SSHing through Tmux through my Linux personal computer)
- Lambda (used it as Node.js service based to receive user trigger emailing capabilities from a JS static webpage, returns a OK/KO message to static website)
- Combination of AWS API Gateway service with SES (AWS email service) to allow contact Form capabilities within an otherwise static S3 website
- RDS (for MySQL community)
- S3 (stored a static website on it, and using it to store app uploaded user images instead of storing them on a MySQL "traditional" DB --> would be a bad practice)
- Beanstalk (for deploying Docker containers)
- Route 53 (used it to buy several domains and manage HTTP/HTTPS routings)
- IAM (access control when I was collaborating with other users)
- EventBridge (implented "rules" to turn ON/OFF my EC2 instance on schedule, to reduce costs)
- AWS CodePipeline (including CodeBuild) for the CI/CD (both of my side projects are wrapped in it)

<br>

- <img alt="Azure" src="https://img.shields.io/badge/microsoft%20azure-0089D6?style=for-the-badge&logo=microsoft-azure&logoColor=white"/>
(Microsoft Azure certified + experience with Databricks --> used py Koalas in the context of a Spark cluster)

## Other stuff

- Cron, SSH, Git, daily usage of linux command line


<b>Workflow and agility: </b>
- <img alt="Docker" src="https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white"/>
- <img alt="Jenkins" src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=Jenkins&logoColor=white"/> (using it as a nice Linux Cron, to orchestrate my autonomous python jobs on EC2)


<b>OS': </b>
- <img alt="MS" src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white"/> (the main OS I'm using)
- <img alt="Ubuntu" src="https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white"/>

<br>

## How to reach me: 

<br>
<a href="https://www.linkedin.com/in/alexandre-nesovic-627004144">
<img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>

or: alex@financial-portfolio.io




