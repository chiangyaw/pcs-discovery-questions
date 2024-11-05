# Prisma Cloud Discovery Questions
## Introduction
This is a general guideline to help partners to run through a discovery, to determine whether a customer has a need for Prisma Cloud, or whether there is any particular pain point that Prisma Cloud can help customer to solve.

### Business & Cloud Discovery 
1. What is driving customer to utilize the cloud (e.g. datacenter migration, new apps, AI services, etc.)?
2. What type of applications is the customer running in the cloud? What do these apps do for their business?
E.g. e-commerce app that processes $10M daily transactions.  
3. Does the customer write their own applications or deploy third party applications? What types of applications are they developing/deploying?
4. Do these apps process customer data, sensitive data, business transactions etc.?
5. What is the business / financial impact to the company if these apps/workloads were compromised (Data exfil, DoS, cryptomining, ransomware, etc)?   Whose jobs would be impacted?
6. What are the Cloud Service Providers (CSPs) in use? AWS, Azure, GCP, Alibaba, Oracle, etc?
7. What are the cloud security problems the customer wants to solve?  Why?  How do they prioritize these problems?
8. What security tools are currently in use?  How are they working? Are there gaps?

### Organization Discovery
1. Who is responsible for building, deploying, and securing these apps in the cloud? In house? Contractors? Outsourced?
2. Walk me through how apps are built.  What teams? How many developers are responsible for building these apps?  How many security people are responsible for these apps?
3. How do developers & security working together to solve security problems?  

### Environment Discovery
1. What % of customer cloud apps are "lift & shift" vs. "cloud native"?
2. What's the release cadence of applications? How often are they moving new code to production
3. What is the workload portfolio (questions below)? 
    - What % of workloads run on VMs, containers, or serverless?   
    - What type of workloads run on these (e.g., e-commerce, web content serving, money transfer, stock trading, analytics)?
    - For VMs, Linux vs. Windows.
    - For containers, which orchestrators (e.g., Managed Kube like AKS, ECS, EKS, GKE, or Self-managed Kube like OpenShift)?
4. Which programming languages are cloud applications written in?  (e.g. Java, JavaScript, Python, Go etc.)
5. Which data services are in use? Do they contain sensitive data like PII, financial information, health care, and other proprietary data like source code etc?
    - Cloud-native ones like AWS S3, RDS, Azure SQL, GCP Cloud Storage, etc
    - Snowflake, Databricks, etc.?
    - Databases installed on cloud-hosted VMs?
6. Which development tools are in use?
    - IDE (e.g Visual Studio, IntelliJ)
    - Git (e.g. GitHub, GitLab, Bitbucket)
    - CICD (e.g., Jenkins, Azure DevOps, Bamboo, CircleCI)
    - Registry for container images (e.g. ACR, GCR, ECR, JFrog) 
7. What % of Cloud Infrastructure is IAC? How does the customer deploy infrastructure in the cloud?
    - Click-Ops - Manual click-click-click on management consoles
    - Infrastructure-as-Code (IAC) (e.g., Terraform, AWS CFT, Azure Resource Management templates/Bicep)
8. Which existing systems/tools do we need to integrate with?  How are they used?
    - IDP / SSO
    - Notification systems (e.g. Jira, Email, PagerDuty, Slack)
    - Ticketing systems (e.g. ServiceNow)
    - SOAR (e.g. XSOAR)
    - SIEM

### Security Process Discovery
1. What metrics are rolled up for security and cloud security? How does the customer measure improvement?
2. Does security have a  "Shift Left" intiative and have "security gates" throughout the software development process at IDE, Git, CICD, Registries to prevent security issues from getting deployed into production?  If not, why not?
3. What's the current alert resolution process?
    - Runtime alerts like misconfig, vuln, threats etc.
    - DevSecops alerts like misconfig, vuln, Application Code, secrets etc. in Git, CICD & Registries
4. How long does it take for a production security alert to get routed to the right Development team and then the right Engineer to identify the right repo and the exact thing to fix?
5. What are the reporting needs?
    - Audience
    - Goal
    - Frequency
    - Delivery format
6. Are there concerns/focus on developer productivity impacted by security?  For example, how many hours is each developer spending per week dealing with production security issues (e.g. misconfig, vuln, threats)?  Those hours could have been spent on building your business applications etc. instead.
7. How do the Cloud Security & SOC teams work together?
8. How do the Cloud Security & Vulnerability Management teams work together?
9. What compliance standards and control frameworks need to be managed to/reported on? HIPAA, PCI DSS, FISMA, OSHA, CIS, ISO, etc

### Licensing Questions
Refer [here](https://github.com/chiangyaw/prismacloudlicensequestionaire).

## Summary
This is just a general guideline on the information that is required to determine whether there is a need for a solution like Prisma Cloud. 