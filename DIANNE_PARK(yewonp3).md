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

--

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

* **Step 1 / Week 1:** Define the core objectives of the MapEdu platform, identifying key social issues related to education and safety in Chicago. Initial datasets from public sources, such as Chicago Public Schools and police beat records, are collected for exploratory review.

* **Step 2 / Week 2:** Conduct thorough data cleaning, including handling missing values, normalizing formats, and checking spatial accuracy. Merge relevant datasets using spatial joins to prepare a unified geospatial foundation for mapping.

* **Step 3 / Week 3:** Finalize the data schema and establish consistent coordinate systems for geographic mapping. Begin building initial visual prototypes to test data visibility and layering between education and safety data.

In weeks four through seven, the focus shifts to visualization development. The team evaluates different visualization libraries, builds interactive charts, and integrates filters and tooltips to support user exploration. During this stage, the prototype is tested with selected users from different target groups, and feedback is used to refine the design.

* **Step 4 / Week 4:** Evaluate and experiment with different data visualization libraries such as Altair, Bqplot, and Folium to determine the most effective tools for interactive mapping. Develop initial mockups to assess feasibility and aesthetics.

* **Step 5 / Week 5:** Create and refine core visualizations including school locations, beat boundaries, and incident overlays. Integrate interactive components such as filters, tooltips, and hover details to improve user engagement.

* **Step 6 / Week 6:** Conduct usability testing sessions with a small group of target users (e.g., parents, planners, researchers) to collect qualitative feedback. Identify pain points and technical issues based on real user interaction.

* **Step 7 / Week 7:** Iterate on the design based on testing insights, making improvements to navigation, visual clarity, and interactivity. Refactor code to ensure modularity and streamline the user experience.

In the final three weeks, the project is deployed using Streamlit. Documentation is completed and published to ensure that new users and contributors can quickly understand and contribute to the platform. By following this phased workflow, MapEdu maintains agility while ensuring thorough development and testing.

* **Step 8 / Week 8:** Begin platform deployment using Streamlit, configuring the server environment for reliability and responsiveness. Resolve any deployment-related bugs or compatibility issues.

* **Step 9 / Week 9:** Draft comprehensive user and developer documentation, including setup guides, data source explanations, and contribution guidelines to support open-source collaboration.

* **Step 10 / Week 10:** Final testing and polish phase—review all platform components for stability, responsiveness, and clarity. Launch the final version of MapEdu and promote the repository for public access and collaboration via GitHub.


### Project Governance and Sustainability
MapEdu adopts a structured but open approach to project governance. A core team of maintainers is responsible for reviewing pull requests, resolving issues, and maintaining the project roadmap. These maintainers are expected to rotate responsibilities to avoid burnout and promote knowledge transfer.

To sustain long-term development, MapEdu explores partnerships with civic technology organizations, educational institutions, and grant-funding bodies. By building a network of collaborators and supporters, the project can access funding, resources, and user feedback critical for long-term success.

Transparency is a core value. Regular updates on progress, challenges, and community metrics are shared through project newsletters or blog posts. This ensures accountability and builds trust with the user and contributor base.

### Future Expansion and Impact
As the platform matures, several paths for expansion are envisioned. MapEdu aims to include additional data types such as environmental quality metrics, public transportation accessibility, and housing data. By layering these datasets, users can gain deeper insights into the structural conditions that affect educational and safety outcomes.

The platform also seeks to expand geographically, integrating data from other U.S. cities and eventually international regions. This would allow cross-border comparisons and help highlight best practices or disparities in resource distribution.

MapEdu’s impact extends beyond software. By conducting workshops and creating educational content, the project will promote open data literacy and community engagement. These efforts support a more informed public and foster a culture of data transparency.

### Conclusion
MapEdu is not just a mapping platform—it is a tool for civic empowerment. By integrating education and safety data into a single, accessible interface and grounding the project in open-source and working open principles, MapEdu seeks to democratize urban data and promote equity. Its modular architecture, community-oriented design, and transparent governance make it a model for future civic tech projects. As the project grows, it will continue to evolve in response to community needs, technological advancements, and new opportunities for collaboration.
