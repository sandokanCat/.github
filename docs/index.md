# Documentation index

This is the repository's catalogued documentation index. The repository is a reusable GitHub community-health and configuration repository, not a single application. Some listed documents are planned templates or placeholders; a listed path is not, by itself, an active policy. Use populated, relevant documents as authoritative sources.

## Primary entry points

- [Repository overview](../README.md) — repository purpose and scope.
- [Canonical agent instructions](../AGENTS.md) — project-wide instructions for coding agents.
- [AI instruction architecture](./ai/AGENT_ARCHITECTURE.md) — compatibility model, discovery caveats, and adapter policy.
- `Contribution guide` — contribution workflow and documentation conventions.
- [Development summary](../SUMMARY.md) — commit work log grouped by UTC date and logical type.
- [Changelog](../CHANGELOG.md) — notable changes by release.
- [Version record](../VERSION.md) — current release or prerelease scope and status.
- [Decision register](./decisions/DECISIONS.md) — durable team decisions.
- [Release process](./releases/RELEASE_PROCESS.md) — release preparation and publication.
- [Tagging conventions](./releases/TAGGING.md) — version tags and immutable release anchors.
- [Release checklist](./releases/RELEASE_CHECKLIST.md) — final release checks.

## Catalogued documentation

## 1. Project identity, introduction and status

- [OVERVIEW.md](./docs/identity/OVERVIEW.md) – Overview of the system, its objectives and components.
- [ABOUT.md](./docs/identity/ABOUT.md) – Background information on the project.
- [PROJECT.md](./docs/identity/PROJECT.md) – Description of the scope, purpose and limitations.
- [PROJECT_STATUS.md](./docs/identity/PROJECT_STATUS.md) – Current status, roadblocks and maintenance status.
- [CHANGELOG.md](../CHANGELOG.md) — Curated release changelog following Keep a Changelog.
- [CHANGES.md](../CHANGES.md) — Deprecated; use the [decision register](./decisions/DECISIONS.md).
- [RELEASE_NOTES.md](./docs/releases/RELEASE_NOTES.md) – What’s new in a specific version.
- [ROADMAP.md](./docs/identity/ROADMAP.md) – Planned features and future priorities.
- [FAQ.md](./docs/identity/FAQ.md) – Frequently asked questions.
- [AUTHORS.md](./AUTHORS.md) – Main authors.
- [CONTRIBUTORS.md](./CONTRIBUTORS.md) – People who have contributed to the project.
- [ACKNOWLEDGMENTS.md](./docs/identity/ACKNOWLEDGMENTS.md) – Acknowledgements and additional credits.
- [CITATION.md](./CITATION.md) – Instructions for citing the software.
- [CITATION.cff](./CITATION.cff) – Structured citation metadata.
- [LICENSE.md](./LICENSE.md) – Licence text or explanation.
- [COPYRIGHT.md](./docs/identity/COPYRIGHT.md) – Copyright notices and conditions.
- [DISCLAIMER.md](./docs/identity/DISCLAIMER.md) – Limitations of liability and warnings.
- [NOTICE.md](./NOTICE.md) – Legal notices or third-party attributions.
- [VERSION.md](../VERSION.md) — Expanded record of the current release or prerelease.

## 2. Community, collaboration and contributions

- `CONTRIBUTING.md` – Explains how to contribute, test and submit changes.
- [CODE_OF_CONDUCT.md](./docs/CODE_OF_CONDUCT.md) – Rules of conduct and handling of breaches.
- [SUPPORT.md](./docs/SUPPORT.md) – Channels for obtaining support.
- [SECURITY.md](./docs/SECURITY.md) – Security policy and vulnerability reporting.
- [GOVERNANCE.md](./docs/GOVERNANCE.md) – Governance and decision-making model.
- [MAINTAINERS.md](./docs/community/MAINTAINERS.md) – Maintenance leads and their roles.
- [COMMUNITY.md](./docs/community/COMMUNITY.md) – Resources and guidelines for participating in the community.
- [ONBOARDING.md](./docs/development/ONBOARDING.md) – Onboarding new contributors.
- [COLLABORATION.md](./docs/community/COLLABORATION.md) – Collaboration agreements and practices.
- [MAINTENANCE.md](./docs/community/MAINTENANCE.md) – Regular project maintenance tasks.
- [FUNDING.md](./docs/community/FUNDING.md) – Explains how to support the project financially.
- [CODEOWNERS.md](./docs/community/CODEOWNERS.md) – Explanation of the code ownership system.
- [PULL_REQUEST_TEMPLATE.md](./.github/PULL_REQUEST_TEMPLATE.md) – Explains or supplements the process for submitting pull requests.
- [ISSUE_TEMPLATE.md](./docs/ISSUE_TEMPLATE.md) – General documentation or template for issues.

## 3. Installation, configuration and getting started

- [INSTALL.md](./docs/installation/INSTALL.md) – Installation procedure.
- [INSTALLATION.md](./docs/installation/INSTALLATION.md) – Comprehensive installation guide.
- [SETUP.md](./docs/installation/SETUP.md) – Initial environment setup.
- [GETTING_STARTED.md](./docs/installation/GETTING_STARTED.md) – First steps to start using the project.
- [QUICKSTART.md](./docs/installation/QUICKSTART.md) – Quick guide to getting your first result.
- [CONFIGURATION.md](./docs/installation/CONFIGURATION.md) – Configuration options and their effects.
- [CONFIG.md](./docs/installation/CONFIG.md) – A brief configuration reference.
- [ENVIRONMENT.md](./docs/installation/ENVIRONMENT.md) – Environment requirements and necessary variables.
- [ENVIRONMENT_VARIABLES.md](./docs/installation/ENVIRONMENT_VARIABLES.md) – Environment variables, their meanings and permitted values.
- [PREREQUISITES.md](./docs/installation/PREREQUISITES.md) – Software, permissions or hardware prerequisites.
- [DEPENDENCIES.md](./docs/installation/DEPENDENCIES.md) – Dependencies and known restrictions.
- [DEVELOPMENT.md](./docs/development/DEVELOPMENT.md) – Setting up the development environment.
- [LOCAL_DEVELOPMENT.md](./docs/development/LOCAL_DEVELOPMENT.md) – Local development workflow.
- [FIRST_RUN.md](./docs/installation/FIRST_RUN.md) – First-run procedure.
- [BOOTSTRAP.md](./docs/installation/BOOTSTRAP.md) – Automated initialisation of an environment or project.
- [UPGRADE.md](./docs/installation/UPGRADE.md) – Updating an installation.
- [UPGRADING.md](./docs/installation/UPGRADING.md) – Upgrade procedures, typically between versions.
- [UNINSTALL.md](./docs/installation/UNINSTALL.md) – Uninstallation and clean-up.
- [TROUBLESHOOTING.md](./docs/installation/TROUBLESHOOTING.md) – Troubleshooting issues during setup or execution.

## 4. Building, compiling and packaging

- [BUILD.md](./docs/build/BUILD.md) – Compilation instructions.
- [BUILDING.md](./docs/development/BUILDING.md) – Detailed guide to compiling from source code.
- [COMPILATION.md](./docs/build/COMPILATION.md) – Compilation procedures and requirements.
- [BUILD_SYSTEM.md](./docs/architecture/BUILD_SYSTEM.md) – Explanation of the build system.
- [PACKAGING.md](./docs/build/PACKAGING.md) – Creation and structure of distributable packages.
- [DISTRIBUTION.md](./docs/build/DISTRIBUTION.md) – Distribution channels and formats.
- [ARTIFACTS.md](./docs/build/ARTIFACTS.md) – Generated artefacts and where they are produced.
- [CROSS_COMPILATION.md](./docs/development/CROSS_COMPILATION.md) – Compilation for different architectures or platforms.
- [TOOLCHAIN.md](./docs/development/TOOLCHAIN.md) – Compilers, SDKs and required tools.
- [BUILD_MATRIX.md](./docs/build/BUILD_MATRIX.md) – Combinations of systems, compilers and compatible versions.
- [REPRODUCIBLE_BUILDS.md](./docs/security/REPRODUCIBLE_BUILDS.md) – How to achieve reproducible and verifiable builds.
- [BINARY_RELEASES.md](./docs/releases/BINARY_RELEASES.md) – Generating and publishing binaries.
- [SOURCE_RELEASES.md](./docs/releases/SOURCE_RELEASES.md) – Preparing source code packages.
- [INSTALL_FROM_SOURCE.md](./docs/installation/INSTALL_FROM_SOURCE.md) – Installation by compiling from source code.

## 5. Deployment, release and operations

- [DEPLOY.md](./docs/deployment/DEPLOY.md) – Specific steps for deployment.
- [DEPLOYMENT.md](./docs/operations/DEPLOYMENT.md) – Deployment architecture and strategy.
- [DEPLOYMENT_GUIDE.md](./docs/deployment/DEPLOYMENT_GUIDE.md) – Detailed deployment guide.
- [RELEASE.md](./docs/releases/RELEASE.md) – Preparing and releasing a version.
- [RELEASING.md](./docs/operations/RELEASING.md) – Repeatable procedure for releasing versions.
- [PUBLISHING.md](./docs/operations/PUBLISHING.md) – Publishing packages, libraries or documentation.
- [PRODUCTION.md](./docs/operations/PRODUCTION.md) – Specifics of the production environment.
- [STAGING.md](./docs/operations/STAGING.md) – Configuration of the pre-production environment.
- [OPERATIONS.md](./docs/operations/OPERATIONS.md) – Routine operations and system maintenance.
- [RUNBOOK.md](./docs/operations/RUNBOOK.md) – Repeatable operational procedures.
- [MONITORING.md](./docs/operations/MONITORING.md) – Metrics, alerts and monitoring.
- [OBSERVABILITY.md](./docs/operations/OBSERVABILITY.md) – Logs, metrics, traces and system diagnostics.
- [LOGGING.md](./docs/operations/LOGGING.md) – Log configuration and handling.
- [BACKUP.md](./docs/operations/BACKUP.md) – Backups and restoration.
- [RESTORE.md](./docs/operations/RESTORE.md) – Data recovery from backups.
- [DISASTER_RECOVERY.md](./docs/operations/DISASTER_RECOVERY.md) – Recovery following major failures.
- [ROLLBACK.md](./docs/operations/ROLLBACK.md) – Rolling back to a previous version or configuration.
- [INCIDENT_RESPONSE.md](./docs/operations/INCIDENT_RESPONSE.md) – Operational response to incidents.
- [CAPACITY_PLANNING.md](./docs/operations/CAPACITY_PLANNING.md) – Resource estimation and capacity planning.
- [SCALING.md](./docs/operations/SCALING.md) – Scaling procedures.
- [MAINTENANCE_WINDOW.md](./docs/operations/MAINTENANCE_WINDOW.md) – Maintenance windows and operational restrictions.
- [SERVICE_LEVELS.md](./docs/operations/SERVICE_LEVELS.md) – Availability targets and service levels.
- [SLO.md](./docs/operations/SLO.md) – Service level objectives.
- [SLA.md](./docs/operations/SLA.md) – Service Level Agreements.

## 6. Architecture, design and technical decisions

- [ARCHITECTURE.md](./docs/architecture/ARCHITECTURE.md) – Architecture overview.
- [SYSTEM_ARCHITECTURE.md](./docs/architecture/SYSTEM_ARCHITECTURE.md) – Overall system architecture.
- [DESIGN.md](./docs/architecture/DESIGN.md) – Technical or functional design.
- [TECHNICAL_DESIGN.md](./docs/design/TECHNICAL_DESIGN.md) – Detailed technical design.
- [SPEC.md](./docs/specs/SPEC.md) – Specification of a function or system.
- [SPECIFICATION.md](./docs/specs/SPECIFICATION.md) – Requirements and expected behaviour.
- [REQUIREMENTS.md](./docs/architecture/REQUIREMENTS.md) – Functional and non-functional requirements.
- [ADR.md](./docs/adr/ADR.md) – General document or index of architectural decisions.
- [RFC.md](./docs/rfcs/RFC.md) – Technical proposal requiring discussion or review.
- [DECISIONS.md](./docs/decisions/DECISIONS.md) – General record of decisions.
- [DATA_MODEL.md](./docs/architecture/DATA_MODEL.md) – Entities, relationships and data structure.
- [DATABASE.md](./docs/architecture/DATABASE.md) – Database design and operation.
- [SCHEMA.md](./docs/architecture/SCHEMA.md) – Description of a data schema or validation.
- [API_DESIGN.md](./docs/api/API_DESIGN.md) – API design criteria.
- [INTEGRATION_ARCHITECTURE.md](./docs/architecture/INTEGRATION_ARCHITECTURE.md) – Integrations, boundaries and flows between systems.
- [COMPONENTS.md](./docs/architecture/COMPONENTS.md) – Components and responsibilities.
- [MODULES.md](./docs/architecture/MODULES.md) – Modules, interfaces and dependencies.
- [DEPENDENCY_GRAPH.md](./docs/architecture/DEPENDENCY_GRAPH.md) – Relationships and dependencies between components.
- [EVENT_MODEL.md](./docs/architecture/EVENT_MODEL.md) – Events, producers, consumers and contracts.
- [STATE_MACHINE.md](./docs/design/STATE_MACHINE.md) – States and transitions within a system.
- [SEQUENCE_DIAGRAMS.md](./docs/architecture/SEQUENCE_DIAGRAMS.md) – Temporal interactions between components.
- [DESIGN_SYSTEM.md](./docs/design/DESIGN_SYSTEM.md) – Visual principles, tokens and interface components.
- [UI_ARCHITECTURE.md](./docs/architecture/UI_ARCHITECTURE.md) – Structure of the interface and its components.
- [ADR-0001.md](./docs/adr/ADR-0001.md) – Individual record of an architectural decision.
- [RFC-0001.md](./docs/rfcs/RFC-0001.md) – Individual technical proposal.

## 7. APIs, protocols and integrations

- [API.md](./docs/api/API.md) – Overview of the API.
- [API_REFERENCE.md](./docs/api/API_REFERENCE.md) – Reference for endpoints, parameters and responses.
- [API_GUIDE.md](./docs/api/API_GUIDE.md) – Practical guide to using an API.
- [REST_API.md](./docs/api/REST_API.md) – Specific features of a REST API.
- [GRAPHQL.md](./docs/api/GRAPHQL.md) – Using the GraphQL schema and queries.
- [WEBSOCKETS.md](./docs/api/WEBSOCKETS.md) – Communication via WebSocket.
- [WEBHOOKS.md](./docs/api/WEBHOOKS.md) – Outgoing events, payloads, signatures and retries.
- [AUTHENTICATION.md](./docs/security/AUTHENTICATION.md) – Authentication mechanisms.
- `AUTHORISATION.md` – Permissions and access control.
- [ERROR_CODES.md](./docs/api/ERROR_CODES.md) – Error catalogue for an API or library.
- [RATE_LIMITING.md](./docs/api/RATE_LIMITING.md) – Request limits and handling of excess requests.
- [PAGINATION.md](./docs/api/PAGINATION.md) – Paginating conventions.
- [VERSIONING.md](./docs/api/VERSIONING.md) – Versioning strategy for the API or library.
- [COMPATIBILITY.md](./docs/api/COMPATIBILITY.md) – Compatibility between clients, versions and platforms.
- [INTEGRATIONS.md](./docs/integrations/INTEGRATIONS.md) – External services and integration mechanisms.
- [PLUGINS.md](./docs/api/PLUGINS.md) – The plugin system and how to develop plugins.
- [EXTENSIONS.md](./docs/api/EXTENSIONS.md) – Available extensions and how to implement them.
- [ADAPTERS.md](./docs/architecture/ADAPTERS.md) – Adapters, contracts and interfaces.
- [SDK.md](./docs/sdk/SDK.md) – Using an SDK.
- [CLIENT_LIBRARIES.md](./docs/api/CLIENT_LIBRARIES.md) – Supported client libraries.
- [MCP.md](./docs/integrations/MCP.md) – Designing or using a Model Context Protocol integration.
- [PROTOCOL.md](./docs/api/PROTOCOL.md) – Proprietary or implemented communication protocol.
- [OPENAPI.md](./docs/api/OPENAPI.md) – How the OpenAPI specification is used in the project.
- [SCHEMA_REGISTRY.md](./docs/architecture/SCHEMA_REGISTRY.md) – Registration and management of schemas.

## 8. Testing, quality and code maintenance

- [TESTING.md](./docs/testing/TESTING.md) – How to run tests.
- [TEST_PLAN.md](./docs/testing/TEST_PLAN.md) – Scope, strategy and test criteria.
- [TEST_STRATEGY.md](./docs/testing/TEST_STRATEGY.md) – Overall approach to quality and testing.
- [UNIT_TESTS.md](./docs/testing/UNIT_TESTS.md) – Running and organising unit tests.
- [INTEGRATION_TESTS.md](./docs/testing/INTEGRATION_TESTS.md) – Tests between components.
- [E2E_TESTING.md](./docs/testing/E2E_TESTING.md) – End-to-end testing.
- [ACCEPTANCE_TESTING.md](./docs/testing/ACCEPTANCE_TESTING.md) – Acceptance criteria and tests.
- [QA.md](./docs/testing/QA.md) – Quality assurance procedures.
- [QUALITY_GATES.md](./docs/development/QUALITY_GATES.md) – Conditions that a change must meet before being integrated or released.
- [CODE_STYLE.md](./docs/development/CODE_STYLE.md) – Code style and conventions.
- [STYLE_GUIDE.md](./docs/testing/STYLE_GUIDE.md) – Code, writing or interface style guide.
- [CODING_STANDARDS.md](./docs/development/CODING_STANDARDS.md) – Implementation rules.
- [LINTING.md](./docs/development/LINTING.md) – Linting tools and how to run them.
- [FORMATTING.md](./docs/development/FORMATTING.md) – Automatic code formatting.
- [DEBUGGING.md](./docs/development/DEBUGGING.md) – Debugging techniques and tools.
- [PROFILING.md](./docs/performance/PROFILING.md) – Analysis of CPU, memory and other resources.
- [BENCHMARKS.md](./docs/performance/BENCHMARKS.md) – Methodology and results of performance tests.
- [PERFORMANCE.md](./docs/testing/PERFORMANCE.md) – Performance and optimisation considerations.
- [REFACTORING.md](./docs/development/REFACTORING.md) – Refactoring criteria and procedures.
- [TECHNICAL_DEBT.md](./docs/testing/TECHNICAL_DEBT.md) – Known technical debt and pending improvements.
- [KNOWN_ISSUES.md](./docs/testing/KNOWN_ISSUES.md) – Known issues and limitations.
- [DEPRECATIONS.md](./docs/testing/DEPRECATIONS.md) – Deprecated features and alternatives.
- [FLAKY_TESTS.md](./docs/testing/FLAKY_TESTS.md) – Unreliable tests and corrective measures.
- [TEST_DATA.md](./docs/testing/TEST_DATA.md) – Preparation, sourcing and management of test data.
- [COVERAGE.md](./docs/testing/COVERAGE.md) – Objectives and interpretation of code coverage.
- [MUTATION_TESTING.md](./docs/testing/MUTATION_TESTING.md) – Mutation testing methodology.

## 9. Security, privacy and compliance

- [SECURITY_POLICY.md](./docs/security/SECURITY_POLICY.md) – Broader security policy.
- [THREAT_MODEL.md](./docs/security/THREAT_MODEL.md) – Assets, threats, attack surfaces and mitigations.
- [SECURE_DEVELOPMENT.md](./docs/security/SECURE_DEVELOPMENT.md) – Secure development practices.
- [SECURITY_ARCHITECTURE.md](./docs/security/SECURITY_ARCHITECTURE.md) – Security controls and architecture.
- [VULNERABILITY_DISCLOSURE.md](./docs/security/VULNERABILITY_DISCLOSURE.md) – Responsible disclosure procedure.
- [ACCESS_CONTROL.md](./docs/security/ACCESS_CONTROL.md) – Roles, permissions and access rules.
- [ENCRYPTION.md](./docs/security/ENCRYPTION.md) – Use of encryption and cryptographic decisions.
- [KEY_MANAGEMENT.md](./docs/security/KEY_MANAGEMENT.md) – Key generation, custody, rotation and revocation.
- [SECRETS_MANAGEMENT.md](./docs/security/SECRETS_MANAGEMENT.md) – Management of secrets and credentials.
- [PRIVACY.md](./docs/privacy/PRIVACY.md) – Privacy considerations and data processing.
- [DATA_PROTECTION.md](./docs/privacy/DATA_PROTECTION.md) – Data protection measures.
- [DATA_RETENTION.md](./docs/privacy/DATA_RETENTION.md) – Data retention and deletion.
- [DATA_CLASSIFICATION.md](./docs/security/DATA_CLASSIFICATION.md) – Classification of data by sensitivity.
- [COMPLIANCE.md](./docs/compliance/COMPLIANCE.md) – Compliance requirements and applicable controls.
- [AUDIT.md](./docs/security/AUDIT.md) – Scope or results of an audit.
- [SECURITY_AUDIT.md](./docs/security/SECURITY_AUDIT.md) – Technical security audit.
- [PENTEST.md](./docs/security/PENTEST.md) – Scope and methodology of a penetration test.
- [SBOM.md](./docs/security/SBOM.md) – Explanation of the software component inventory.
- [SUPPLY_CHAIN_SECURITY.md](./docs/security/SUPPLY_CHAIN_SECURITY.md) – Software supply chain risks.
- [DEPENDENCY_SECURITY.md](./docs/security/DEPENDENCY_SECURITY.md) – Audit and management of vulnerable dependencies.
- [CRYPTOGRAPHY.md](./docs/security/CRYPTOGRAPHY.md) – Cryptographic design and algorithms used.
- [ABUSE_CASES.md](./docs/security/ABUSE_CASES.md) – Abuse cases and associated controls.
- [RISK_ASSESSMENT.md](./docs/security/RISK_ASSESSMENT.md) – Risk identification and assessment.

## 10. User guides, tutorials and educational material

- [USER_GUIDE.md](./docs/user-guide/USER_GUIDE.md) – Comprehensive user guide.
- [ADMIN_GUIDE.md](./docs/guides/ADMIN_GUIDE.md) – Software operation and administration.
- [USAGE.md](./docs/guides/USAGE.md) – Instructions for use and basic examples.
- [TUTORIAL.md](./docs/tutorials/TUTORIAL.md) – Step-by-step practical tutorial.
- [TUTORIALS.md](./docs/guides/TUTORIALS.md) – Index of tutorials.
- [EXAMPLES.md](./docs/examples/EXAMPLES.md) – Usage examples.
- [COOKBOOK.md](./docs/guides/COOKBOOK.md) – Recipes for common tasks.
- [CLI.md](./docs/guides/CLI.md) – Using the command-line interface.
- [COMMANDS.md](./docs/cli/COMMANDS.md) – Command reference.
- [GLOSSARY.md](./docs/guides/GLOSSARY.md) – Definitions of terms.
- [LIMITATIONS.md](./docs/guides/LIMITATIONS.md) – Unsupported features and known limitations.
- [MIGRATION_GUIDE.md](./docs/migration/MIGRATION_GUIDE.md) – Detailed migration guide.
- [HOW_IT_WORKS.md](./docs/guides/HOW_IT_WORKS.md) – Conceptual explanation of how it works.
- [CONCEPTS.md](./docs/guides/CONCEPTS.md) – Fundamental concepts of the system.
- [RECIPES.md](./docs/guides/RECIPES.md) – A collection of practical solutions.
- [BEST_PRACTICES.md](./docs/guides/BEST_PRACTICES.md) – Best practices.
- [ANTI_PATTERNS.md](./docs/guides/ANTI_PATTERNS.md) – Practices to avoid and the reasons why.
- [CHEATSHEET.md](./docs/guides/CHEATSHEET.md) – Summary of commands or concepts for quick reference.
- [GLOSSARY_OF_TERMS.md](./docs/guides/GLOSSARY_OF_TERMS.md) – Comprehensive technical glossary.
- [FAQ_DEVELOPERS.md](./docs/development/FAQ_DEVELOPERS.md) – Frequently asked questions for developers.
- [FAQ_USERS.md](./docs/user-guide/FAQ_USERS.md) – Frequently asked questions for users.
- [ACCESSIBILITY.md](./docs/ACCESSIBILITY.md) – Accessibility guide or criteria for accessible use.
- `LOCALISATION.md` – How to add languages and translate the application.
- [TRANSLATION.md](./docs/guides/TRANSLATION.md) – Translation workflow and string management.

## 11. Project management, planning and decision-making

- [PLAN.md](./docs/project/PLAN.md) – Implementation or development plan.
- [TODO.md](./docs/project/TODO.md) – Tasks to be done.
- [TASKS.md](./docs/project/TASKS.md) – Task breakdown.
- [MILESTONES.md](./docs/project/MILESTONES.md) – Milestones and verifiable objectives.
- [PROGRESS.md](./docs/project/PROGRESS.md) – Progress tracking.
- [MEETING_NOTES.md](./docs/meetings/MEETING_NOTES.md) – Meeting minutes or notes.
- [POSTMORTEM.md](./docs/postmortems/POSTMORTEM.md) – Analysis of an incident or failure that has already occurred.
- [LESSONS_LEARNED.md](./docs/project/LESSONS_LEARNED.md) – Lessons learnt from the project.
- [HANDOVER.md](./docs/operations/HANDOVER.md) – Transfer of responsibilities or knowledge.
- [STAKEHOLDERS.md](./docs/project/STAKEHOLDERS.md) – Stakeholders and their responsibilities.
- [PROJECT_CHARTER.md](./docs/project/PROJECT_CHARTER.md) – Project objectives, scope, authority and framework.
- [RISK_REGISTER.md](./docs/project/RISK_REGISTER.md) – Risk register, probability, impact and mitigation.
- [ASSUMPTIONS.md](./docs/project/ASSUMPTIONS.md) – Planning assumptions and hypotheses.
- [SCOPE.md](./docs/project/SCOPE.md) – Included and excluded scope.
- [CHANGE_REQUESTS.md](./docs/project/CHANGE_REQUESTS.md) – Procedure for requesting and assessing changes.
- [DEFINITION_OF_DONE.md](./docs/development/DEFINITION_OF_DONE.md) – Criteria for considering a task complete.
- [DEFINITION_OF_READY.md](./docs/development/DEFINITION_OF_READY.md) – Criteria for considering a task ready.
- [WORKFLOW.md](./docs/project/WORKFLOW.md) – General workflow for the team or project.
- [PROCESS.md](./docs/project/PROCESS.md) – Operational or development process.
- [PRIORITIES.md](./docs/project/PRIORITIES.md) – Criteria and order of priorities.
- [SUPPORT_MODEL.md](./docs/operations/SUPPORT_MODEL.md) – Support model and responsibilities.

## 12. Versioning, release and compatibility

- [SEMANTIC_VERSIONING.md](./docs/releases/SEMANTIC_VERSIONING.md) – How semantic versioning is applied.
- [RELEASE_PROCESS.md](./docs/releases/RELEASE_PROCESS.md) – Complete release process.
- [RELEASE_CHECKLIST.md](./docs/releases/RELEASE_CHECKLIST.md) – Pre-release checklist.
- [MIGRATION.md](./docs/migration/MIGRATION.md) – Changes required when migrating.
- [BREAKING_CHANGES.md](./docs/releases/BREAKING_CHANGES.md) – Breaking changes and their implications.
- [DEPRECATION_POLICY.md](./docs/releases/DEPRECATION_POLICY.md) – Deprecation policy.
- [SUPPORT_POLICY.md](./docs/releases/SUPPORT_POLICY.md) – Supported versions policy.
- [COMPATIBILITY_MATRIX.md](./docs/releases/COMPATIBILITY_MATRIX.md) – Matrix of compatible versions, platforms or dependencies.
- [LIFECYCLE.md](./docs/releases/LIFECYCLE.md) – Version or component lifecycle.
- [LTS.md](./docs/releases/LTS.md) – Long-term support policy.
- [BACKPORTS.md](./docs/releases/BACKPORTS.md) – Criteria for incorporating fixes into previous branches.
- [HOTFIX.md](./docs/releases/HOTFIX.md) – Procedure for urgent fixes.
- [BRANCHING_STRATEGY.md](./docs/development/BRANCHING_STRATEGY.md) – Git branching strategy.
- [TAGGING.md](./docs/releases/TAGGING.md) – Conventions for Git tags.
- [CHANGE_MANAGEMENT.md](./docs/releases/CHANGE_MANAGEMENT.md) – Change assessment, approval and control.

## 13. Infrastructure, networking and systems documentation

- [INFRASTRUCTURE.md](./docs/infrastructure/INFRASTRUCTURE.md) – Infrastructure inventory and architecture.
- [INFRASTRUCTURE_OVERVIEW.md](./docs/infrastructure/INFRASTRUCTURE_OVERVIEW.md) – Overview of resources and services.
- [NETWORK.md](./docs/infrastructure/NETWORK.md) – Network design and operation.
- [NETWORKING.md](./docs/infrastructure/NETWORKING.md) – Network and communications configuration.
- [DNS.md](./docs/operations/DNS.md) – DNS configuration and name resolution.
- [TLS.md](./docs/security/TLS.md) – TLS certificate configuration and renewal.
- [CERTIFICATES.md](./docs/security/CERTIFICATES.md) – Certificate lifecycle management.
- [FIREWALL.md](./docs/infrastructure/FIREWALL.md) – Firewall rules and design.
- [CONTAINERS.md](./docs/infrastructure/CONTAINERS.md) – Container usage and architecture.
- [DOCKER.md](./docs/infrastructure/DOCKER.md) – Building, running and configuring Docker.
- [KUBERNETES.md](./docs/infrastructure/KUBERNETES.md) – Deployment and operation on Kubernetes.
- [HELM.md](./docs/infrastructure/HELM.md) – Using Helm charts and configuration.
- [TERRAFORM.md](./docs/infrastructure/TERRAFORM.md) – Organising and using Terraform.
- [INFRASTRUCTURE_AS_CODE.md](./docs/infrastructure/INFRASTRUCTURE_AS_CODE.md) – Principles and workflow of infrastructure as code.
- [CLOUD_ARCHITECTURE.md](./docs/architecture/CLOUD_ARCHITECTURE.md) – Cloud services architecture.
- [AWS.md](./docs/infrastructure/AWS.md) – AWS-specific configuration or architecture.
- [AZURE.md](./docs/infrastructure/AZURE.md) – Azure-specific configuration or architecture.
- [GCP.md](./docs/infrastructure/GCP.md) – Google Cloud-specific configuration or architecture.
- [RESOURCE_LIMITS.md](./docs/operations/RESOURCE_LIMITS.md) – Limits on CPU, memory, storage or other resources.
- [STORAGE.md](./docs/infrastructure/STORAGE.md) – Storage design and operation.
- [HIGH_AVAILABILITY.md](./docs/architecture/HIGH_AVAILABILITY.md) – Redundancy and fault tolerance.
- [NETWORK_SECURITY.md](./docs/security/NETWORK_SECURITY.md) – Segmentation, network controls and risks.
- [ENVIRONMENT_TOPOLOGY.md](./docs/infrastructure/ENVIRONMENT_TOPOLOGY.md) – Relationship between environments and their resources.

## 14. Data, databases and processing

- [DATABASE_SCHEMA.md](./docs/data/DATABASE_SCHEMA.md) – Database schema.
- [MIGRATIONS.md](./docs/data/MIGRATIONS.md) – Database migration management.
- [SEEDING.md](./docs/data/SEEDING.md) – Initial data loading.
- [DATA_IMPORT.md](./docs/data/DATA_IMPORT.md) – Data import.
- [DATA_EXPORT.md](./docs/data/DATA_EXPORT.md) – Data export.
- [DATA_VALIDATION.md](./docs/data/DATA_VALIDATION.md) – Data validation and integrity rules.
- [DATA_QUALITY.md](./docs/data/DATA_QUALITY.md) – Data quality, consistency and completeness.
- [DATA_PIPELINE.md](./docs/data/DATA_PIPELINE.md) – Processing and transformation flow.
- [ETL.md](./docs/data/ETL.md) – Extraction, transformation and loading.
- [DATA_LINEAGE.md](./docs/data/DATA_LINEAGE.md) – Data provenance and transformations.
- [DATA_DICTIONARY.md](./docs/data/DATA_DICTIONARY.md) – Definition of fields, types and meanings.
- [DATA_GOVERNANCE.md](./docs/data/DATA_GOVERNANCE.md) – Responsibilities, policies and data quality.
- [BACKUP_STRATEGY.md](./docs/operations/BACKUP_STRATEGY.md) – Data backup and recovery strategy.
- [RETENTION_POLICY.md](./docs/data/RETENTION_POLICY.md) – Data retention and disposal.
- [DATA_PRIVACY.md](./docs/privacy/DATA_PRIVACY.md) – Privacy considerations in data processing.
- [ANALYTICS.md](./docs/data/ANALYTICS.md) – Instrumentation, product metrics and analytics.
- [DATA_WAREHOUSE.md](./docs/data/DATA_WAREHOUSE.md) – Data warehouse architecture.
- [STREAMING.md](./docs/data/STREAMING.md) – Streaming data processing.
- [DATA_FORMATS.md](./docs/data/DATA_FORMATS.md) – Supported data formats.

## 15. Documentation for AI tools and programming assistants

- [AGENTS.md](./AGENTS.md) – Instructions and context for supported programming agents.
- [CLAUDE.md](./CLAUDE.md) – Persistent instructions for Claude Code.
- [GEMINI.md](./GEMINI.md) – Context and instructions for Gemini CLI.
- [copilot-instructions.md](./.github/copilot-instructions.md) – General GitHub Copilot instructions for the repository.
- [project.instructions.md](./.github/instructions/project.instructions.md) – Copilot instructions with a specific scope based on your configuration (representative placeholder for the documented filename pattern).
- [SKILL.md](./SKILL.md) – Defines a reusable skill for specific agents.
- [PROMPT.md](./docs/ai/PROMPT.md) – Reusable prompt or instructions for a task.
- [PROMPTS.md](./prompts/PROMPTS.md) – Catalogue of prompts.
- [AI_GUIDELINES.md](./docs/ai/AI_GUIDELINES.md) – Guidelines for using AI in the project.
- [AI_POLICY.md](./docs/ai/AI_POLICY.md) – AI usage policy.
- [CONTEXT.md](./docs/ai/CONTEXT.md) – Context of an agent or automated process.
- [MODEL_CARD.md](./docs/ai/MODEL_CARD.md) – Information about a model, its capabilities and limitations.
- [EVALUATION.md](./docs/ai/EVALUATION.md) – Methodology for evaluating models or agents.
- [EVALS.md](./docs/ai/EVALS.md) – Set or methodology of automated evaluations.
- [GUARDRAILS.md](./docs/ai/GUARDRAILS.md) – Restrictions and controls for an AI system.
- [TOOLING.md](./docs/development/TOOLING.md) – Tools available to the agent or team.
- [AGENT_ARCHITECTURE.md](./docs/ai/AGENT_ARCHITECTURE.md) – Architecture of an agent or multi-agent system.

## 16. Site documentation, manuals and documentation generators

- `index.md` – Home page for a documentation section.
- [mkdocs.yml](./mkdocs.yml) – MkDocs site configuration.
- [DOCS.md](./docs/documentation/DOCS.md) – Table of contents or overview of the available documentation.
- [DOCUMENTATION.md](./docs/documentation/DOCUMENTATION.md) – General guide to the project’s documentation.
- [DOCUMENTATION_GUIDE.md](./docs/documentation/DOCUMENTATION_GUIDE.md) – Guidelines for writing and maintaining documentation.
- [WRITING_GUIDE.md](./docs/documentation/WRITING_GUIDE.md) – Technical writing guidelines.
- [INFORMATION_ARCHITECTURE.md](./docs/documentation/INFORMATION_ARCHITECTURE.md) – Organisation of information and navigation.
- [DOCS_ARCHITECTURE.md](./docs/documentation/DOCS_ARCHITECTURE.md) – Internal organisation of the documentation system.
- [VERSIONED_DOCS.md](./docs/documentation/VERSIONED_DOCS.md) – Version management for documentation.
- [TRANSLATION_GUIDE.md](./docs/documentation/TRANSLATION_GUIDE.md) – Document translation process.
- [DOCS_DEPLOYMENT.md](./docs/operations/DOCS_DEPLOYMENT.md) – Publication of the documentation site.
- [DOCS_MAINTENANCE.md](./docs/documentation/DOCS_MAINTENANCE.md) – Documentation maintenance and review.

## 17. Legal documentation, licences and policies

- [TERMS.md](./docs/legal/TERMS.md) – Terms of use.
- [TERMS_OF_SERVICE.md](./docs/legal/TERMS_OF_SERVICE.md) – Terms of service.
- [PRIVACY_POLICY.md](./docs/legal/PRIVACY_POLICY.md) – Privacy policy.
- [COOKIE_POLICY.md](./docs/legal/COOKIE_POLICY.md) – Cookie policy.
- [ACCEPTABLE_USE_POLICY.md](./docs/policies/ACCEPTABLE_USE_POLICY.md) – Permitted and prohibited uses.
- [DATA_PROCESSING.md](./docs/privacy/DATA_PROCESSING.md) – Processing of personal data.
- [DATA_PROCESSING_AGREEMENT.md](./docs/legal/DATA_PROCESSING_AGREEMENT.md) – Terms and conditions governing data processing between parties.
- [THIRD_PARTY_NOTICES.md](./docs/legal/THIRD_PARTY_NOTICES.md) – Third-party attributions and notices.
- [EXPORT_CONTROL.md](./docs/legal/EXPORT_CONTROL.md) – Export control considerations.
- [ETHICS.md](./docs/policies/ETHICS.md) – Ethical principles of the project.
- [ACCESSIBILITY_POLICY.md](./docs/policies/ACCESSIBILITY_POLICY.md) – Accessibility policy.

## 18. Scientific research, reproducibility and academic documentation

- [RESEARCH.md](./docs/research/RESEARCH.md) – Research context and research questions.
- [METHODOLOGY.md](./docs/research/METHODOLOGY.md) – Methodology used.
- [EXPERIMENTS.md](./docs/research/EXPERIMENTS.md) – Design and record of experiments.
- [REPRODUCIBILITY.md](./docs/research/REPRODUCIBILITY.md) – How to reproduce results or experiments.
- [DATASET.md](./docs/data/DATASET.md) – Description of a dataset.
- [DATASET_CARD.md](./docs/data/DATASET_CARD.md) – Origin, composition, limitations and uses of a dataset.
- [EXPERIMENT_LOG.md](./docs/research/EXPERIMENT_LOG.md) – Record of experiments.
- [RESULTS.md](./docs/research/RESULTS.md) – Results obtained and their interpretation.
- [ETHICS_STATEMENT.md](./docs/research/ETHICS_STATEMENT.md) – Ethical considerations of a research project.
- [RESEARCH_QUESTIONS.md](./docs/research/RESEARCH_QUESTIONS.md) – Research questions and hypotheses.
- [BIBLIOGRAPHY.md](./docs/research/BIBLIOGRAPHY.md) – Bibliography in human-readable format.
- [REFERENCES.md](./docs/research/REFERENCES.md) – References and sources.
- [REPLICATION_GUIDE.md](./docs/research/REPLICATION_GUIDE.md) – Instructions for replicating a study.

## 19. Product, user experience and accessibility

- [PRODUCT.md](./docs/product/PRODUCT.md) – Product vision and purpose.
- [PRODUCT_REQUIREMENTS.md](./docs/product/PRODUCT_REQUIREMENTS.md) – Product requirements.
- [PRD.md](./docs/product/PRD.md) – Product Requirements Document.
- [USER_STORIES.md](./docs/product/USER_STORIES.md) – User stories and requirements.
- [PERSONAS.md](./docs/product/PERSONAS.md) – Target user profiles.
- [USER_FLOWS.md](./docs/design/USER_FLOWS.md) – User flows.
- [UX.md](./docs/design/UX.md) – User experience guidelines.
- [UI.md](./docs/design/UI.md) – Interface design and implementation.
- [BRANDING.md](./docs/design/BRANDING.md) – Visual identity, tone and brand usage.
- [CONTENT_GUIDELINES.md](./docs/product/CONTENT_GUIDELINES.md) – Content and microcopy guidelines.
- [EXPERIMENTATION.md](./docs/product/EXPERIMENTATION.md) – A/B testing and product experiments.
- [FEATURE_FLAGS.md](./docs/operations/FEATURE_FLAGS.md) – Use and management of toggleable features.
- [FEEDBACK.md](./docs/product/FEEDBACK.md) – Channels and process for collecting feedback.
- [USER_RESEARCH.md](./docs/research/USER_RESEARCH.md) – Methodology and results of user research.
- [INTERNATIONALIZATION.md](./docs/product/INTERNATIONALIZATION.md) – Architecture and process for internationalisation.

## 20. Domain-specific documentation

- [BLOCKCHAIN.md](./docs/architecture/BLOCKCHAIN.md) – Architecture and integration with blockchain.
- [SMART_CONTRACTS.md](./docs/contracts/SMART_CONTRACTS.md) – Organisation, interfaces and behaviour of smart contracts.
- [TOKENOMICS.md](./docs/domain/TOKENOMICS.md) – Economic design of tokens.
- [CONSENSUS.md](./docs/architecture/CONSENSUS.md) – Consensus algorithm or mechanism.
- [WALLETS.md](./docs/domain/WALLETS.md) – Wallet management and integration.
- [RPC.md](./docs/domain/RPC.md) – RPC interfaces and node configuration.
- [NODE_OPERATIONS.md](./docs/operations/NODE_OPERATIONS.md) – Installation, maintenance and operation of nodes.
- [MINING.md](./docs/domain/MINING.md) – Mining design and operation, where applicable.
- [VALIDATORS.md](./docs/domain/VALIDATORS.md) – Validator operation and responsibilities.
- [DEFI.md](./docs/domain/DEFI.md) – Architecture of decentralised finance applications.

## Existing GitHub and documentation configuration

- [sidebars.js](./sidebars.js) – Configuration of the side navigation in Docusaurus.

- [Docusaurus configuration](./docusaurus.config.js) – Configuration for a Docusaurus documentation site.
- [Issue template configuration](./.github/ISSUE_TEMPLATE/config.yml) – GitHub issue template selector and contact links.
- [Bug report template](./.github/ISSUE_TEMPLATE/bug_report.yml) – Structured bug reports.
- [Feature request template](./.github/ISSUE_TEMPLATE/feature_request.yml) – Structured feature proposals.
- [Discussion: ideas](./.github/DISCUSSION_TEMPLATE/ideas.yml) – Template for discussions about ideas.
- [Discussion: Q&A](./.github/DISCUSSION_TEMPLATE/q-a.yml) – Template for questions and answers.
- [Vulnerability report configuration](./.github/VULNERABILITY_REPORT.yml) – Existing placeholder for vulnerability-reporting configuration.
- [GitHub funding configuration](./.github/FUNDING.yml) – Sponsor and funding links.
- [CODEOWNERS](./docs/CODEOWNERS) – Existing code ownership file at a GitHub-supported location.
