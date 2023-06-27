## Values

[We have them!](./values.md)

## Special Interest Groups (SIGs)

In our platform engineering project, we organize our teams and work efforts into Special Interest Groups (SIGs). Each SIG focuses on a specific area or function of the platform and is composed of members from various teams and organizations. The purpose of SIGs is to advance the platform in their respective domains, promote code ownership, and facilitate collaboration among contributors. Each identifiable component or aspect of the project, including repositories, APIs, tests, and issues, is assigned to a specific SIG.

SIGs can cover vertical topics that are specific to certain components or functions, horizontal topics that span multiple functional areas, or topics related to supporting the project itself. Here are some examples:

- Vertical SIGs: Network, Infrastructure Automation, CI/CD, Security and Compliance, Cloud Management, Observability (Monitoring and Logging)
- Horizontal SIGs: Scalability, Architecture
- Project SIGs: Testing, Release Management, Documentation, Contributor Experience

Each SIG is led by one or ideally two SIG chairs who serve as organizers and facilitators. They are responsible for managing the SIG's operations, coordinating with other SIGs, the Steering Committee, and the wider community.

To ensure clarity and accountability, each SIG must have a charter that outlines its scope, responsibilities, areas of authority, member selection process, decision-making procedures, and conflict resolution mechanisms. The charter defines the SIG's operating guidelines while allowing flexibility for customization within broad community guidelines and constraints.

While much of the work within a SIG is conducted internally, it is essential to maintain open communication. SIGs should document meeting notes, discussions, designs, and decisions to ensure transparency and accessibility for other SIGs and community members. Regular summaries of the SIG's work should be shared with the broader community.

For more details on SIG governance, including mailing lists and meeting schedules, refer to the SIG Governance Requirements. The SIG Lifecycle provides a tactical checklist for SIG creation and retirement.

## Subprojects

Within each SIG, specific work efforts are divided into subprojects. Every aspect of our platform, including infrastructure, automation, CI/CD pipelines, security and compliance measures, cloud management, and observability, is assigned to a subproject within the corresponding SIG. Subprojects may have distinct sets of contributors and technical leaders who are responsible for guiding the vision, direction, and overall design of the subproject. They also approve change proposals (KEPs), address technical escalations, and contribute to the subproject's success.

Here are some examples of subprojects within SIGs:

- SIG Network: Pod networking (CNI, etc.), Service (including kube-proxy), Ingress, DNS, Network policy
- SIG Infrastructure Automation: Terraform automation, infrastructure provisioning templates, configuration management
- SIG CI/CD: Pipeline automation, build and deployment tools integration, automated testing frameworks
- SIG Security and Compliance: Access controls, encryption, vulnerability scanning, compliance frameworks
- SIG Cloud Management: Cloud infrastructure provisioning, optimization, cost management
- SIG Observability: Monitoring solutions, logging frameworks, performance analysis tools

To learn more about the subprojects within each SIG, refer to the sigs.yaml documentation.

By structuring our platform engineering efforts into SIGs and subprojects, we create focused forums for collaboration, distributed decision-making, and code ownership. This approach allows us to effectively advance our platform, ensure accountability, and foster a vibrant and inclusive community of contributors.

## Cross-project Communication and Coordination

While most work shouldn’t require expensive coordination with other SIGs, there will be efforts (features, refactoring, etc.) that cross SIG boundaries. In this case, it is expected that the SIGs coordinate with each other and come to mutually agreed solutions. In some cases, it may make sense to form a Working Group for joint work. Cross-SIG coordination will naturally require more time and implies a certain amount of overhead. This is intentional to encourage changes to be well encapsulated whenever possible.

On the other hand, several SIGs do have project-wide impact, for example Release, Testing, and API Machinery. Even those that do not may sometimes need to make changes or impose new processes or conventions that affect other SIGs. In these cases, project-wide communication processes will need to be followed. For example, proposals with project-wide impact will need to be announced more broadly, with the opportunity for members of other SIGs to provide feedback and guidance. However, the SIG that owns the area, according to its charter, will own the decision. 

The [PEP](./peps) process facilitates definition, agreement and communication of efforts that cross SIG boundaries. SIGs are encouraged to use this process for larger efforts. This process is also available for smaller efforts within a SIG.