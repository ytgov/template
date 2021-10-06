

# Guide for Publishing Open Source Code 
 
It is recommended that where they have the right to do so, departments publish all source code as open source software, whether the software solution was (i) acquired as OSS; (ii) developed in-house by YG employees or (iii) acquired through the terms of procurement contracts where appropriate license terms were negotiated. 
 
When releasing the code at large is not appropriate, or possible, it is recommended to start with sharing the source code internally to all departments, to the extent that the terms of the applicable license permit such sharing. Care should be taken to ensure that the license to Yukon does not limit the distribution of such code to specified user departments. Doing so will help make the source code ready to be released publicly as open source where Yukon has received the right to do so. 
 
The steps to publish source code are: 
1. [Seek Approvals](#seek-approvals)
2. [Consider Security Implications](#consider-security-implications)
3. [Select Open Source Software Licence](#select-open-source-software-license) 
4. [Create Source Code Repository](#Create-Source-Code-Repository)
5. [Add Recommended Files](#add-recommended-files) 
6. [Publishing a Legacy Application](#publishing-a-legacy-application) 
7. [Work in the Open](#work-in-open) 
 
## 1. Seek Approvals 
 > To review for alignment with YG processes and structures
### Team 
The Directive on Management of IT support the Digital Standard #3: Working in the open by default, via Mandatory Procedures for Enterprise Architecture Assessment (C2.3.8). 

Share evidence, research and decision making openly. Make all non-sensitive data, information, and new code developed in delivery of services open to the outside world for sharing and reuse under an open licence. 

Aligned with the Open Government vision, teams should by default consider adapting their process to develop as open source from the inception of projects to reduce the overhead required to release their source code later down the road. 
It has also been found that doing so improves the quality of the code developed and encourages collaboration. 
 
### Department 
Similar to open data or information covered by the Directive on Open Government, the publication of source code under an open source software licence, requires appropriate department or agency approvals. 

That person may vary according to your department and delegation should be encouraged to the lowest level possible to encourage the release of open source code. 
 
## 2. Consider Security Implications 
 
### Developing Software in the Open 
- Keep sensitive data such as credentials secure and separate from source code. 
Avoid storing keys and other sensitive material in systems not approved for that purpose. 
- Code reviews increase the likelihood of catching bugs, security vulnerabilities, and reduces the risk of committing sensitive data. 
Implement controls sufficient to prevent unauthorized or inadvertent changes such as code signing and repository user rights. 
- Develop mitigation strategies and processes to address security related incidents. 
- Embed security practices in your daily processes and methodologies. 
- Leverage tools and services to automate finding known security vulnerabilities, - possible secret keys and personally identifiable information. 
 
## 3. Select Open Source Software Licence 
When the project is part of a larger open source software community, like plugins, modules, extensions, or derivative works of existing open source software, it is highly recommended to use the license which is usually used by the community. 
 
When the project is started by Yukon itself and isn’t related to an external community, the choice of the open source licence has to be based off of the licences of the components (3rd party libraries and framework) you will use and the desired outcome. 
 
*Recommended permissive licences* 
 
**MIT**

*When to use:* Small, simple projects and scripts. 

[Licence text MIT ](https://opensource.org/licenses/MIT)
 
**Apache 2.0**

*When to use:* Larger software project use Apache 2.0 because it provides a grant of patents. 

[Licence text  Apache2.0 ](http://www.apache.org/licenses/LICENSE-2.0.txt)
 
*Recommended reciprocal licences*
 
**GPL 3.0 or later**
*When to use*: Software 
[Licence text  ‘GPL 3.0 or later’](https://www.gnu.org/licenses/gpl-3.0.txt)
 
**LGPL 3.0 or later**
*When to use:* Libraries 
[Licence text  ‘LGPL 3.0 or later’](https://www.gnu.org/licenses/lgpl-3.0.txt)
 
**AGPL 3.0 or later** 
*When to use:* Web applications and services 
[Licence text  ‘AGPL 3.0 or later’](https://www.gnu.org/licenses/agpl-3.0.txt) 
 
### Applying a License 
To apply to source code, add the text of the chosen licence to a LICENSE.txt file in the root folder of the project. See Add Recommended Files. You could also just add the licence text directly in one of your source code file but by making it clearly available at the root of your project, you make it easier for people to find it and some collaboration platforms can automatically display your licence in the web interface. 
 
If multiple licences can be applied, choose a licence which matches the goal of the project and its interactions with other projects. This tends to revolve around the decision of whether to apply a permissive or reciprocal licence. 
 
### Copyright
> To review.  Yukon may take a different position on copyright

The Canadian Copyright Act (section 12) provides that where any work is, or has been, prepared or published by or under the direction or control of Her Majesty or any government department, the copyright in the work shall, subject to any agreement with the author, belong to Her Majesty. This applies to source code developed by Government of Canada employees. 

However, Government of Canada employees have Moral Rights and as the author of a work has the right to the integrity of the work and the right to be associated with the work as its author by name or under a pseudonym and the right to remain anonymous. 
 
### Appropriate Yukon government Copyright Identification 
> To review.  Yukon may take a different position on copyright

As per the Crown Copyright Request article found on Canada.ca, the following structure should be applied for the Government of Canada Copyright notice. 
Copyright (c) Her Majesty the Queen in Right of Canada, as represented by the Minister of (legal departmental name), (year of publication). 

Replace the (legal departmental name) and (year of publication) with the appropriate information. 

This notice should be added to the LICENCE file in your project. See Add Recommended Files 
 
## Create Source Code Repository 
 
Recommended public source code repositories for Yukon government open source code are: 
- [GitHub](https://github.com/ytgov) 
 
Yukon government also has an internal source code repository available to all departments and agencies. 
- GitLab (internal to Yukon Government only) 
 
### Organizations 
Departments and agencies are free to choose the platform that best suits their operational needs but their projects should, where possible, all be regrouped under a unique organization or group. This would help discoverability of your projects but also help increase collaboration opportunities. 
 
### Version Control System 
The recommended version control system for YG open source code is Git. Departments are also encouraged to use Git to manage their source code internally. 
 
### Add Recommended Files 
Before publishing, source code should include the following file: 
a LICENCE (see Select Open Source Software Licence) file containing a copy of the licence under which the source code is released; 
 
Note: the open source licence itself can be applied in the source code directly but it is highly recommended to put it in a separate LICENCE file at the root of your project directory. 
 
Additionally, the following are recommended as best practice: 
- a README.md file providing information about the project, how to use it and general - documentation. 
- It is also recommended that this file be bilingual to increase use and contribution - to the project. 
- a CONTRIBUTING.md file explaining how to contribute to the project. 
- a SECURITY.md file explaining security policy as well as procedures for reporting - security vulnerabilities. 
- a CODE_OF_CONDUCT.md file explaining the values and ethics for the public sector employees and for the project. 
Examples of these files are available in the Template Repository. 
 
## Publishing a Legacy Application 
Publishing a legacy application can seem like a lot of work but it is feasible and actually a good investment if the application will continue to be used in the future. Documentation could be improved during the release project to help increase community contributions. 
 
Additionally, releasing a legacy application may lead to reuse and increase in development contributions from interested parties. It may revive the active development of the application, providing it with enhanced features and bug fixes. 
Vulnerability risks already exist and releasing it as open source doesn’t change their state. One way of limiting those risks is to not provide the configurations of the production version. 
 
Scanning tools with advanced functionalities and security tests should be considered to help the development teams speed up the review and clean up process. 
 
## Work in the Open 
 
### Release Early, Release Often 
It is recommended that the source code be released as early as possible in the project’s life cycle to avoid the overhead of publishing source code late in the process. The public source code repository is encouraged to be the single source of truth where developers are working. The latest code version may not necessarily mean it’s the version deployed in production. 
 
### You’re In Control 
When working in the open teams still have control over what makes it into the source code and a chance to review contributions from internal and external developers. Access rights can be configured for repositories to ensure only authorized team members can accept changes. Others may distribute modified version of your code, but it doesn’t mean the changes have to be accepted as part of your code. 
 
## Identify as an employee of the Yukon Government 
Employees should use their full name and Yukon government email address for all code contributions to public repositories while acting within the scope of their duties or employment. 
 
## Community 
Building a welcoming community can influence your project’s future and reputation. By providing a positive experience for contributors and making it easy for them to interact with the project team, you encourage them to keep coming back and contributing. You should respond to questions, bugs and merge requests to encourage people to continue helping you. 
 
It is recommended to include a README.md and CONTRIBUTING.md file with your source code. See Add Recommended Files. 
 
## Contributor License Agreement 
Yukon Government projects don’t require contributor license agreements, but rely on the open source software licenses providing the necessary terms. Contributions are made under the same license under which the project is released and that authors retain their copyright for their contributions. 
 
## Attribution
This guide is adapted from: https://www.canada.ca/en/government/system/digital-government/digital-government-innovations/open-source-software/guide-for-publishing-open-source-code.html 
