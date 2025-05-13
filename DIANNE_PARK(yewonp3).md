## MapEdu: Mapping Education and Safety

Author: Dianne Park (yewonp3)

Course & Semester: SP25 IS 340 Final Paper

Presentation Link: https://www.canva.com/design/DAGmuRsnwgQ/g9TP-6St3wkoNX1VjdPaAg/view?utm_content=DAGmuRsnwgQ&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h0b7ed930c5

---

### Abstract

Access to education and community safety are foundational aspects of urban development, yet understanding their interplay often remains inaccessible to everyday citizens and policymakers. "MapEdu" is a hypothetical open-source project that seeks to address this gap by providing an interactive data visualization platform that overlays public education data with community safety metrics. While the initial scope is centered on the city of Chicago, the platform is designed to be scalable, adaptable, and inclusive of additional datasets and geographies. This paper outlines the vision, management strategies, technical structure, and open-source principles that guide the development of MapEdu.

---

### Project Objectives and Vision
The core objective of MapEdu is to empower stakeholders with data-driven insights on the relationship between education infrastructure and public safety. Chicago communities, like many urban environments, often lack accessible and integrated information on how educational and safety resources are distributed. MapEdu seeks to solve this by creating a unified platform that visualizes public school locations alongside police beat boundaries. This will assist city planners and school administrators with resource allocation and support families and researchers in evaluating neighborhood dynamics.

In the long-term, MapEdu envisions expansion beyond the city of Chicago. The goal is to incorporate additional datasets, such as transportation infrastructure, healthcare accessibility, or economic indicators, and to scale the platform to include higher education facilities and international data. Through this expansion, MapEdu aims to serve as a global resource for understanding urban equity.

### Target User Profiles
MapEdu has been designed with four primary user groups in mind. First, city planners will benefit from integrated spatial data that enables more equitable and informed policy decisions. These users need tools that help them visualize the overlap of educational facilities and police jurisdictions to better allocate funding and services. Second, school administrators can use MapEdu to understand how school zones intersect with safety jurisdictions, helping them to coordinate with public safety agencies more effectively. Third, prospective parents and students often consider both safety and education quality when choosing where to live. MapEdu will provide them with easy-to-access and reliable data visualizations to support their decision-making. Lastly, researchers focused on urban policy, education, and social equity will find the platform a valuable tool for analyzing correlations and trends across public service domains.

### Open Source Development Strategy
The technical foundation of MapEdu relies on a suite of widely adopted open-source tools. For data processing, Python is the core language, supplemented by the Pandas library for handling tabular data and GeoPandas for spatial data analysis. These tools offer robust functionality, a wide community support base, and flexibility necessary for handling diverse and evolving datasets.

Data visualization is accomplished through libraries such as Altair and Bqplot. These Python-based tools allow the development team to build interactive, customizable visualizations that can be easily integrated into the data pipeline. The visual interface will allow users to explore educational facilities and crime statistics in a single, intuitive dashboard.

To streamline front-end development, Streamlit is employed to deploy the user interface. Streamlit’s simple syntax and ease of integration with Python make it a suitable choice for building and iterating quickly without the complexity of traditional web development frameworks.

Lastly, the project is hosted on GitHub, which serves as a centralized platform for version control, collaborative development, and public transparency. GitHub enables the project to be open for contributions, issue tracking, and continuous integration practices.

### Working Open Principles
MapEdu is guided by principles of transparency, collaboration, and inclusivity that are at the heart of the "working open" philosophy. All code is maintained with Git and shared via GitHub, with branching strategies and pull request reviews used to manage code integrity and collaboration.

To ensure usability and sustainability, the project features extensive documentation. This includes user guides, developer setup instructions, and API references. These resources are updated regularly and structured to support both novice contributors and experienced developers.

The platform is released under an open-source license, such as MIT or GPL, allowing users to freely reuse, adapt, and build upon the software. Contributor guidelines and a code of conduct ensure a welcoming and respectful community. Furthermore, community engagement is maintained through public forums, issue discussions, and periodic virtual meetings to review the roadmap and gather feedback.

### Technical Debts and Mitigation Strategies
Like many software projects, MapEdu faces challenges associated with technical debt. These challenges are categorized into three main phases: initial development, long-term maintenance, and mitigation planning.

In the initial development phase, the team anticipates difficulties with dependency management, particularly ensuring that open-source libraries used in the project are compatible and stable across versions. Another challenge lies in data synchronization. Because datasets from educational and public safety sources may update at different rates or in inconsistent formats, maintaining alignment will require ongoing development effort. Additionally, usability testing across different user groups must be prioritized to ensure that the platform meets diverse accessibility and interaction needs.

Over a five-year outlook, other sources of technical debt may arise. Software libraries such as Streamlit or GeoPandas could evolve, introducing breaking changes that affect platform functionality. Performance bottlenecks may also emerge as the volume and variety of data grow, especially if the project expands to other cities or begins handling real-time data. Moreover, scalability becomes a concern if the platform gains a large user base, which may exceed the capabilities of the current hosting infrastructure.

To mitigate these risks, MapEdu employs version pinning to stabilize the development environment, ensuring that library updates do not unexpectedly break the system. A modular codebase allows individual components to be updated independently, improving maintainability. The platform is designed with cloud hosting in mind, making it easier to migrate to services like AWS or Azure when demand increases. Finally, robust documentation and internal code comments reduce the project’s reliance on any single contributor’s knowledge.

### Development Workflow and Timeline

| ![](https://github.com/OREL-group/Project-Management/blob/e3269b8d32d8f9e1d260021f91f7445136e3a028/FINAL%20PAPERS/IS%20340%20Workflow.png) | 
| :--: |
| <b>Figure 1.</b> Caption test. [Store image as an issue](https://github.com/OREL-group/Project-Management/issues/279) or in the local directory. |   

The project’s development is structured over a 10-week timeline, divided into three key phases. During the first three weeks, the team focuses on defining project objectives and gathering data from publicly available sources. This phase involves cleaning, standardizing, and integrating datasets using spatial joins to align school locations with police beat boundaries.

In weeks four through seven, the focus shifts to visualization development. The team evaluates different visualization libraries, builds interactive charts, and integrates filters and tooltips to support user exploration. During this stage, the prototype is tested with selected users from different target groups, and feedback is used to refine the design.

In the final three weeks, the project is deployed using Streamlit. Documentation is completed and published to ensure that new users and contributors can quickly understand and contribute to the platform. By following this phased workflow, MapEdu maintains agility while ensuring thorough development and testing.

[Comment_5]: <> (begin your text here)

__Paragraph heading__         

[Comment_6]: <> (begin your text two spaces after the last underscore in the previous line)


### Conclusion      

[Comment_7]: <> (begin your text here)


### References     

[Comment_8]: <> (begin your reference list here. Cite as author, year in main text. Reference link should correpond with link in Comment 2  Use any format you wish -- MLA, APA, etc.)

Cite as the form (Lastname, 2023) in the body of your text. List reference citation in this section. 



[Comment_1]: <> (begin your text here)
[Comment_2]: <> (An example of a reference in paper text, cite in Reference list -- see Comment 8)
#### Subheading
[Comment_3]: <> (begin your text here)

| ![](https://user-images.githubusercontent.com/38323286/233691025-55deb1db-3e35-4589-8c55-4f859f8e41cd.jpg) | 
| :--: |
| <b>Figure 1.</b> Caption test. [Store image as an issue](https://github.com/OREL-group/Project-Management/issues/279) or in the local directory. |   

[Comment_4]: <> (Insert Figure with caption here)
