# MapEdu: Mapping Education and Safety

#### Author: Dianne Park (yewonp3)
#### Course & Semester: SP25 IS 340 Final Paper
#### Presentation Link: https://www.canva.com/design/DAGmuRsnwgQ/g9TP-6St3wkoNX1VjdPaAg/view?utm_content=DAGmuRsnwgQ&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h0b7ed930c5

---

## Abstract

Access to education and community safety are foundational aspects of urban development, yet understanding their interplay often remains inaccessible to citizens and policymakers. "MapEdu" is a hypothetical open-source project that addresses this gap by providing an interactive data visualization platform that overlays public education data with community safety metrics. While the initial scope is centered on Chicago, the platform is designed to be scalable, adaptable, and inclusive of additional datasets and geographies. This paper outlines the vision, management strategies, technical structure, and open-source principles that guide the development of MapEdu.


## Project Objectives and Vision

The core objective of MapEdu is to empower stakeholders with data-driven insights on the relationship between education infrastructure and public safety. Like many urban environments, Chicago communities often lack accessible and integrated information on how educational and safety resources are distributed. MapEdu seeks to solve this by creating a unified platform that visualizes public school locations alongside police beat boundaries. This will assist city planners and school administrators in allocating resources and supporting users in evaluating neighborhood dynamics.

In the long term, MapEdu envisions expansion beyond the city of Chicago. The goal is to incorporate additional datasets, such as transportation infrastructure, healthcare accessibility, or economic indicators, and to scale the platform to include higher education facilities and international data. Through this expansion, MapEdu aims to serve as a global resource for understanding urban equity.


## Target User Profiles

MapEdu has been designed with four primary user groups in mind. First, city planners will benefit from integrated spatial data that enables more equitable and informed policy decisions. These users need tools that help them visualize the overlap of educational facilities and police jurisdictions to allocate funding and services better. Second, school administrators can use MapEdu to understand how school zones intersect with safety jurisdictions, helping them coordinate more effectively with public safety agencies. Third, prospective parents and students often consider safety and education quality when choosing where to live. MapEdu will provide them with easy-to-access and reliable data visualizations to support their decision-making. Lastly, researchers focused on urban policy, education, and social equity will find the platform valuable for analyzing correlations and trends across public service domains.


## Open Source Development Strategy

The technical foundation of MapEdu relies on a suite of widely adopted open-source tools. Python is the core language for data processing, supplemented by the Pandas library for handling tabular data and GeoPandas for spatial data analysis. These tools offer robust functionality, a broad community support base, and flexibility for handling diverse and evolving datasets. Data visualization is accomplished through libraries such as Altair and Bqplot. These Python-based tools allow the development team to build interactive, customizable visualizations that can be easily integrated into the data pipeline. The visual interface will allow users to explore educational facilities and crime statistics in a single, intuitive dashboard. Streamlit is employed to deploy the user interface to streamline front-end development. Streamlit’s simple syntax and ease of integration with Python make it suitable for building and iterating quickly without the complexity of traditional web development frameworks. Lastly, the project is hosted on GitHub, a centralized platform for version control, collaborative development, and public transparency. GitHub enables the project to be open for contributions, issue tracking, and continuous integration practices.


## Working Open Principles

MapEdu is guided by principles of transparency, collaboration, and inclusivity at the heart of the "working open" philosophy. All code is maintained with Git and shared via GitHub, with branching strategies and pull request reviews used to manage code integrity and collaboration. To ensure usability and sustainability, the project features extensive documentation. This includes user guides, developer setup instructions, and API references. These resources are updated regularly and structured to support novice contributors and experienced developers. The platform is released under an open-source license, such as MIT or GPL, allowing users to freely reuse, adapt, and build upon the software. Contributor guidelines and a code of conduct ensure a welcoming and respectful community. Furthermore, community engagement is maintained through public forums, issue discussions, and periodic virtual meetings to review the roadmap and gather feedback.


## Technical Debts and Mitigation Strategies

Like many software projects, MapEdu faces challenges associated with technical debt. These challenges are categorized into three phases: initial development, long-term maintenance, and mitigation planning.

In the initial development phase, the team anticipates difficulties with dependency management, particularly ensuring that open-source libraries used in the project are compatible and stable across versions. Another challenge lies in data synchronization. Because datasets from educational and public safety sources may update at different rates or in inconsistent formats, maintaining alignment will require ongoing development effort. Additionally, usability testing across different user groups must be prioritized to ensure the platform meets diverse accessibility and interaction needs.

Other sources of technical debt may arise over a five-year outlook. Software libraries such as Streamlit or GeoPandas could evolve, introducing breaking changes that affect platform functionality. Performance bottlenecks may also emerge as the volume and variety of data grow, especially if the project expands to other cities or begins handling real-time data. Moreover, scalability becomes a concern if the platform gains a large user base, which may exceed the capabilities of the current hosting infrastructure.

To mitigate these risks, MapEdu employs version pinning to stabilize the development environment, ensuring that library updates do not unexpectedly break the system. A modular codebase allows individual components to be updated independently, improving maintainability. The platform is designed with cloud hosting in mind, making it easier to migrate to services like AWS or Azure when demand increases. Finally, robust documentation and internal code comments reduce the project’s reliance on any single contributor’s knowledge.

## Development Workflow and Timeline

![](https://github.com/OREL-group/Project-Management/blob/e3269b8d32d8f9e1d260021f91f7445136e3a028/FINAL%20PAPERS/IS%20340%20Workflow.png)

* **Week 1 – Identify Project Scope and Goals**
  
  Define the primary objective of integrating Chicago Public Schools data with Police Beat boundaries to visualize how education and safety resources are distributed. Clarify key visualization features and the intended user base, including policymakers, families, and researchers.

* **Week 2 – Data Acquisition**

  Collect relevant datasets from public resources, including school location data and police jurisdiction data. Review the completeness and update frequency of each dataset to identify any coverage gaps or inconsistencies.

* **Week 3 – Data Cleaning and Preprocessing**

  Ensure consistency across datasets by normalizing formats, correcting missing or inaccurate values, and aligning coordinate systems. Use spatial joins to link school locations with corresponding police beat areas to enable meaningful geographic analysis.

* **Week 4 – Visualization Library Selection**

  Assess potential visualization libraries such as Altair, Bqplot, Folium, and Plotly based on their ability to support interactivity, geographic mapping, and integration with Streamlit. Identify limitations in data rendering or UI flexibility.

* **Week 5 – Build Visualizations and Interactive Features**

  Begin developing core visual elements, including school density maps and beat boundary overlays. Add interactive features such as filters by neighborhood, school type, or safety metric, along with tooltips for incident detail exploration.

* **Week 6 – Usability Testing and Iteration**

  Conduct testing sessions with selected stakeholders, including parents, planners, and researchers. Gather feedback on visual clarity, functionality, and navigation. Refine the platform’s interface and features based on input.

* **Week 7 – Platform Deployment**

  Deploy the platform using Streamlit, ensuring performance stability and responsive interaction. If scalability or concurrency issues are detected, begin planning a transition to a cloud-based solution such as AWS or Azure.

* **Week 8 – Documentation and Support Planning**

  Create detailed user and developer guides to facilitate long-term use and community contributions. Develop a proactive maintenance plan for addressing data updates, dependency upgrades, and feature enhancements as the platform evolves.


## Project Governance and Sustainability

MapEdu adopts a structured but open approach to project governance. A core team of maintainers is responsible for reviewing pull requests, resolving issues, and maintaining the project roadmap. These maintainers must rotate responsibilities to avoid burnout and promote knowledge transfer. MapEdu explores partnerships with civic technology organizations, educational institutions, and grant-funding bodies to sustain long-term development. By building a network of collaborators and supporters, the project can access funding, resources, and user feedback critical for long-term success. Transparency is a core value. Project newsletters or blog posts share weekly updates on progress, challenges, and community metrics. This ensures accountability and builds trust with the user and contributor base.


## Future Expansion and Impact

As the platform matures, several paths for expansion are envisioned. MapEdu aims to include additional data types such as environmental quality metrics, public transportation accessibility, and housing data. By layering these datasets, users can gain deeper insights into the structural conditions that affect educational and safety outcomes. The platform also seeks to expand geographically, integrating data from other U.S. cities and eventually international regions. This would allow cross-border comparisons and help highlight best practices or disparities in resource distribution. MapEdu’s impact extends beyond software. The project will promote open data literacy and community engagement by conducting workshops and creating educational content. These efforts support a more informed public and foster a culture of data transparency.


## Conclusion

MapEdu is not just a mapping platform but a tool for civic empowerment. By integrating education and safety data into a single, accessible interface and grounding the project in open-source and open principles, MapEdu seeks to democratize urban data and promote equity. Its modular architecture, community-oriented design, and transparent governance make it a model for future civic tech projects. As the project grows, it will continue to evolve in response to community needs, technological advancements, and new opportunities for collaboration.

---


### References     

Mozilla Science Lab. (2023). Working open. Mozilla Science Leadership Workshop. https://mozillascience.github.io/open-science-leadership-workshop/01.2-working_open.html

Police Beats Data: https://data.cityofchicago.org/Public-Safety/Boundaries-Police-Beats-current-/aerh-rz74

Chicago School Location Data: https://data.cityofchicago.org/Education/Chicago-Public-Schools-School-Locations-SY1415/3fhj-xtn5
