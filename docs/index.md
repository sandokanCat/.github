# Documentation index

This is the repository's catalogued documentation index. The repository is a reusable GitHub community-health and configuration repository, not a single application. Some listed documents are planned templates or placeholders; a listed path is not, by itself, an active policy. Use populated, relevant documents as authoritative sources.

## Primary entry points

- [INFORMATION_ARCHITECTURE.md](./documentation/INFORMATION_ARCHITECTURE.md) — placement precedence and root-file requirements.

- [README.md](../README.md) — repository purpose and scope.
- [AGENTS.md](../AGENTS.md) — project-wide instructions for coding agents.
- [AGENT_ARCHITECTURE.md](./ai/AGENT_ARCHITECTURE.md) — compatibility model, discovery caveats, and adapter policy.
- [CONTRIBUTING.md](./CONTRIBUTING.md) — contribution workflow and documentation conventions.
- [WORK_LOG.md](./development/WORK_LOG.md) — repository-defined commit work log grouped by UTC date and logical type.
- [CHANGES.md](./CHANGES.md) — parked legacy filename; not an active changelog.
- [SUMMARY.md](./SUMMARY.md) — parked legacy filename; not the documentation index.
- [CHANGELOG.md](../CHANGELOG.md) — notable changes by release.
- [VERSION.md](./releases/VERSION.md) — current release or prerelease scope and status.
- [DECISIONS.md](./decisions/DECISIONS.md) — durable team decisions.
- [RELEASE_PROCESS.md](./releases/RELEASE_PROCESS.md) — release preparation and publication.
- [TAGGING.md](./releases/TAGGING.md) — version tags and immutable release anchors.
- [RELEASE_CHECKLIST.md](./releases/RELEASE_CHECKLIST.md) — final release checks.

## Catalogued documentation

## 1. Project identity, introduction and status

- [site-verification.ini](./identity/templates/site-verification.ini) — illustrative site-verification settings; not an active secret store.

- [OVERVIEW.md](./identity/OVERVIEW.md) – Overview of the system, its objectives and components.
- [ABOUT.md](./identity/ABOUT.md) – Background information on the project.
- [PROJECT.md](./identity/PROJECT.md) – Description of the scope, purpose and limitations.
- [PROJECT_STATUS.md](./identity/PROJECT_STATUS.md) – Current status, roadblocks and maintenance status.
- [CHANGES.md](./CHANGES.md) — Parked legacy filename; future purpose under review.
- [RELEASE_NOTES.md](./releases/RELEASE_NOTES.md) – What’s new in a specific version.
- [ROADMAP.md](./identity/ROADMAP.md) – Planned features and future priorities.
- [FAQ.md](./identity/FAQ.md) – Frequently asked questions.
- [AUTHORS.md](./community/AUTHORS.md) – Main authors.
- [CONTRIBUTORS.md](./community/CONTRIBUTORS.md) – People who have contributed to the project.
- [ACKNOWLEDGMENTS.md](./identity/ACKNOWLEDGMENTS.md) – Acknowledgements and additional credits.
- [CITATION.md](./legal/CITATION.md) – Instructions for citing the software.
- [CITATION.cff](../CITATION.cff) – Structured citation metadata.
- [LICENSE.md](./legal/LICENSE.md) – Licence text or explanation.
- [COPYRIGHT.md](./identity/COPYRIGHT.md) – Copyright notices and conditions.
- [DISCLAIMER.md](./identity/DISCLAIMER.md) – Limitations of liability and warnings.
- [NOTICE.md](./legal/NOTICE.md) – Legal notices or third-party attributions.
- [VERSION.md](./releases/VERSION.md) — Expanded record of the current release or prerelease.

## 2. Community, collaboration and contributions

- [CONTRIBUTING.md](./CONTRIBUTING.md) – Explains how to contribute, test and submit changes.
- [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md) – Rules of conduct and handling of breaches.
- [SUPPORT.md](./SUPPORT.md) – Channels for obtaining support.
- [SECURITY.md](./SECURITY.md) – Security policy and vulnerability reporting.
- [GOVERNANCE.md](./community/GOVERNANCE.md) – Governance and decision-making model.
- [MAINTAINERS.md](./community/MAINTAINERS.md) – Maintenance leads and their roles.
- [COMMUNITY.md](./community/COMMUNITY.md) – Resources and guidelines for participating in the community.
- [ONBOARDING.md](./development/ONBOARDING.md) – Onboarding new contributors.
- [COLLABORATION.md](./community/COLLABORATION.md) – Collaboration agreements and practices.
- [MAINTENANCE.md](./community/MAINTENANCE.md) – Regular project maintenance tasks.
- [FUNDING.md](./community/FUNDING.md) – Explains how to support the project financially.
- [CODEOWNERS.md](./community/CODEOWNERS.md) – Explanation of the code ownership system.
- [PULL_REQUEST_TEMPLATE.md](../.github/PULL_REQUEST_TEMPLATE.md) – Explains or supplements the process for submitting pull requests.
- [ISSUE_TEMPLATE.md](./community/ISSUE_TEMPLATE.md) – General documentation or template for issues.

## 3. Installation, configuration and getting started

- [INSTALL.md](./installation/INSTALL.md) – Installation procedure.
- [INSTALLATION.md](./installation/INSTALLATION.md) – Comprehensive installation guide.
- [SETUP.md](./installation/SETUP.md) – Initial environment setup.
- [GETTING_STARTED.md](./installation/GETTING_STARTED.md) – First steps to start using the project.
- [QUICKSTART.md](./installation/QUICKSTART.md) – Quick guide to getting your first result.
- [CONFIGURATION.md](./installation/CONFIGURATION.md) – Configuration options and their effects.
- [CONFIG.md](./installation/CONFIG.md) – A brief configuration reference.
- [ENVIRONMENT.md](./installation/ENVIRONMENT.md) – Environment requirements and necessary variables.
- [ENVIRONMENT_VARIABLES.md](./installation/ENVIRONMENT_VARIABLES.md) – Environment variables, their meanings and permitted values.
- [PREREQUISITES.md](./installation/PREREQUISITES.md) – Software, permissions or hardware prerequisites.
- [DEPENDENCIES.md](./installation/DEPENDENCIES.md) – Dependencies and known restrictions.
- [DEVELOPMENT.md](./development/DEVELOPMENT.md) – Setting up the development environment.
- [LOCAL_DEVELOPMENT.md](./development/LOCAL_DEVELOPMENT.md) – Local development workflow.
- [FIRST_RUN.md](./installation/FIRST_RUN.md) – First-run procedure.
- [BOOTSTRAP.md](./installation/BOOTSTRAP.md) – Automated initialisation of an environment or project.
- [UPGRADE.md](./installation/UPGRADE.md) – Updating an installation.
- [UPGRADING.md](./installation/UPGRADING.md) – Upgrade procedures, typically between versions.
- [UNINSTALL.md](./installation/UNINSTALL.md) – Uninstallation and clean-up.
- [TROUBLESHOOTING.md](./installation/TROUBLESHOOTING.md) – Troubleshooting issues during setup or execution.

## 4. Building, compiling and packaging

- [BUILD.md](./build/BUILD.md) – Compilation instructions.
- [BUILDING.md](./development/BUILDING.md) – Detailed guide to compiling from source code.
- [COMPILATION.md](./build/COMPILATION.md) – Compilation procedures and requirements.
- [BUILD_SYSTEM.md](./architecture/BUILD_SYSTEM.md) – Explanation of the build system.
- [PACKAGING.md](./build/PACKAGING.md) – Creation and structure of distributable packages.
- [DISTRIBUTION.md](./build/DISTRIBUTION.md) – Distribution channels and formats.
- [ARTIFACTS.md](./build/ARTIFACTS.md) – Generated artefacts and where they are produced.
- [CROSS_COMPILATION.md](./development/CROSS_COMPILATION.md) – Compilation for different architectures or platforms.
- [TOOLCHAIN.md](./development/TOOLCHAIN.md) – Compilers, SDKs and required tools.
- [BUILD_MATRIX.md](./build/BUILD_MATRIX.md) – Combinations of systems, compilers and compatible versions.
- [REPRODUCIBLE_BUILDS.md](./security/REPRODUCIBLE_BUILDS.md) – How to achieve reproducible and verifiable builds.
- [BINARY_RELEASES.md](./releases/BINARY_RELEASES.md) – Generating and publishing binaries.
- [SOURCE_RELEASES.md](./releases/SOURCE_RELEASES.md) – Preparing source code packages.
- [INSTALL_FROM_SOURCE.md](./installation/INSTALL_FROM_SOURCE.md) – Installation by compiling from source code.

## 5. Deployment, release and operations

- [DEPLOY.md](./deployment/DEPLOY.md) – Specific steps for deployment.
- [DEPLOYMENT.md](./operations/DEPLOYMENT.md) – Deployment architecture and strategy.
- [DEPLOYMENT_GUIDE.md](./deployment/DEPLOYMENT_GUIDE.md) – Detailed deployment guide.
- [RELEASE.md](./releases/RELEASE.md) – Preparing and releasing a version.
- [RELEASING.md](./operations/RELEASING.md) – Repeatable procedure for releasing versions.
- [PUBLISHING.md](./operations/PUBLISHING.md) – Publishing packages, libraries or documentation.
- [PRODUCTION.md](./operations/PRODUCTION.md) – Specifics of the production environment.
- [STAGING.md](./operations/STAGING.md) – Configuration of the pre-production environment.
- [OPERATIONS.md](./operations/OPERATIONS.md) – Routine operations and system maintenance.
- [RUNBOOK.md](./operations/RUNBOOK.md) – Repeatable operational procedures.
- [MONITORING.md](./operations/MONITORING.md) – Metrics, alerts and monitoring.
- [OBSERVABILITY.md](./operations/OBSERVABILITY.md) – Logs, metrics, traces and system diagnostics.
- [LOGGING.md](./operations/LOGGING.md) – Log configuration and handling.
- [BACKUP.md](./operations/BACKUP.md) – Backups and restoration.
- [RESTORE.md](./operations/RESTORE.md) – Data recovery from backups.
- [DISASTER_RECOVERY.md](./operations/DISASTER_RECOVERY.md) – Recovery following major failures.
- [ROLLBACK.md](./operations/ROLLBACK.md) – Rolling back to a previous version or configuration.
- [INCIDENT_RESPONSE.md](./operations/INCIDENT_RESPONSE.md) – Operational response to incidents.
- [CAPACITY_PLANNING.md](./operations/CAPACITY_PLANNING.md) – Resource estimation and capacity planning.
- [SCALING.md](./operations/SCALING.md) – Scaling procedures.
- [MAINTENANCE_WINDOW.md](./operations/MAINTENANCE_WINDOW.md) – Maintenance windows and operational restrictions.
- [SERVICE_LEVELS.md](./operations/SERVICE_LEVELS.md) – Availability targets and service levels.
- [SLO.md](./operations/SLO.md) – Service level objectives.
- [SLA.md](./operations/SLA.md) – Service Level Agreements.

## 6. Architecture, design and technical decisions

- [ARCHITECTURE.md](./architecture/ARCHITECTURE.md) – Architecture overview.
- [SYSTEM_ARCHITECTURE.md](./architecture/SYSTEM_ARCHITECTURE.md) – Overall system architecture.
- [DESIGN.md](./architecture/DESIGN.md) – Technical or functional design.
- [TECHNICAL_DESIGN.md](./design/TECHNICAL_DESIGN.md) – Detailed technical design.
- [SPEC.md](./specs/SPEC.md) – Specification of a function or system.
- [SPECIFICATION.md](./specs/SPECIFICATION.md) – Requirements and expected behaviour.
- [REQUIREMENTS.md](./architecture/REQUIREMENTS.md) – Functional and non-functional requirements.
- [ADR.md](./adr/ADR.md) – General document or index of architectural decisions.
- [RFC.md](./rfcs/RFC.md) – Technical proposal requiring discussion or review.
- [DECISIONS.md](./decisions/DECISIONS.md) – General record of decisions.
- [DATA_MODEL.md](./architecture/DATA_MODEL.md) – Entities, relationships and data structure.
- [DATABASE.md](./architecture/DATABASE.md) – Database design and operation.
- [SCHEMA.md](./architecture/SCHEMA.md) – Description of a data schema or validation.
- [API_DESIGN.md](./api/API_DESIGN.md) – API design criteria.
- [INTEGRATION_ARCHITECTURE.md](./architecture/INTEGRATION_ARCHITECTURE.md) – Integrations, boundaries and flows between systems.
- [COMPONENTS.md](./architecture/COMPONENTS.md) – Components and responsibilities.
- [MODULES.md](./architecture/MODULES.md) – Modules, interfaces and dependencies.
- [DEPENDENCY_GRAPH.md](./architecture/DEPENDENCY_GRAPH.md) – Relationships and dependencies between components.
- [EVENT_MODEL.md](./architecture/EVENT_MODEL.md) – Events, producers, consumers and contracts.
- [STATE_MACHINE.md](./design/STATE_MACHINE.md) – States and transitions within a system.
- [SEQUENCE_DIAGRAMS.md](./architecture/SEQUENCE_DIAGRAMS.md) – Temporal interactions between components.
- [DESIGN_SYSTEM.md](./design/DESIGN_SYSTEM.md) – Visual principles, tokens and interface components.
- [UI_ARCHITECTURE.md](./architecture/UI_ARCHITECTURE.md) – Structure of the interface and its components.
- [ADR-0001.md](./adr/ADR-0001.md) – Individual record of an architectural decision.
- [RFC-0001.md](./rfcs/RFC-0001.md) – Individual technical proposal.

## 7. APIs, protocols and integrations

- [API.md](./api/API.md) – Overview of the API.
- [API_REFERENCE.md](./api/API_REFERENCE.md) – Reference for endpoints, parameters and responses.
- [API_GUIDE.md](./api/API_GUIDE.md) – Practical guide to using an API.
- [REST_API.md](./api/REST_API.md) – Specific features of a REST API.
- [GRAPHQL.md](./api/GRAPHQL.md) – Using the GraphQL schema and queries.
- [WEBSOCKETS.md](./api/WEBSOCKETS.md) – Communication via WebSocket.
- [WEBHOOKS.md](./api/WEBHOOKS.md) – Outgoing events, payloads, signatures and retries.
- [AUTHENTICATION.md](./security/AUTHENTICATION.md) – Authentication mechanisms.
- `AUTHORISATION.md` – Permissions and access control.
- [ERROR_CODES.md](./api/ERROR_CODES.md) – Error catalogue for an API or library.
- [RATE_LIMITING.md](./api/RATE_LIMITING.md) – Request limits and handling of excess requests.
- [PAGINATION.md](./api/PAGINATION.md) – Paginating conventions.
- [VERSIONING.md](./api/VERSIONING.md) – Versioning strategy for the API or library.
- [COMPATIBILITY.md](./api/COMPATIBILITY.md) – Compatibility between clients, versions and platforms.
- [INTEGRATIONS.md](./integrations/INTEGRATIONS.md) – External services and integration mechanisms.
- [PLUGINS.md](./api/PLUGINS.md) – The plugin system and how to develop plugins.
- [EXTENSIONS.md](./api/EXTENSIONS.md) – Available extensions and how to implement them.
- [ADAPTERS.md](./architecture/ADAPTERS.md) – Adapters, contracts and interfaces.
- [SDK.md](./sdk/SDK.md) – Using an SDK.
- [CLIENT_LIBRARIES.md](./api/CLIENT_LIBRARIES.md) – Supported client libraries.
- [MCP.md](./integrations/MCP.md) – Designing or using a Model Context Protocol integration.
- [PROTOCOL.md](./api/PROTOCOL.md) – Proprietary or implemented communication protocol.
- [OPENAPI.md](./api/OPENAPI.md) – How the OpenAPI specification is used in the project.
- [SCHEMA_REGISTRY.md](./architecture/SCHEMA_REGISTRY.md) – Registration and management of schemas.

## 8. Testing, quality and code maintenance

- [TESTING.md](./testing/TESTING.md) – How to run tests.
- [TEST_PLAN.md](./testing/TEST_PLAN.md) – Scope, strategy and test criteria.
- [TEST_STRATEGY.md](./testing/TEST_STRATEGY.md) – Overall approach to quality and testing.
- [UNIT_TESTS.md](./testing/UNIT_TESTS.md) – Running and organising unit tests.
- [INTEGRATION_TESTS.md](./testing/INTEGRATION_TESTS.md) – Tests between components.
- [E2E_TESTING.md](./testing/E2E_TESTING.md) – End-to-end testing.
- [ACCEPTANCE_TESTING.md](./testing/ACCEPTANCE_TESTING.md) – Acceptance criteria and tests.
- [QA.md](./testing/QA.md) – Quality assurance procedures.
- [QUALITY_GATES.md](./development/QUALITY_GATES.md) – Conditions that a change must meet before being integrated or released.
- [CODE_STYLE.md](./development/CODE_STYLE.md) – Code style and conventions.
- [STYLE_GUIDE.md](./testing/STYLE_GUIDE.md) – Code, writing or interface style guide.
- [CODING_STANDARDS.md](./development/CODING_STANDARDS.md) – Implementation rules.
- [LINTING.md](./development/LINTING.md) – Linting tools and how to run them.
- [FORMATTING.md](./development/FORMATTING.md) – Automatic code formatting.
- [DEBUGGING.md](./development/DEBUGGING.md) – Debugging techniques and tools.
- [PROFILING.md](./performance/PROFILING.md) – Analysis of CPU, memory and other resources.
- [BENCHMARKS.md](./performance/BENCHMARKS.md) – Methodology and results of performance tests.
- [PERFORMANCE.md](./testing/PERFORMANCE.md) – Performance and optimisation considerations.
- [REFACTORING.md](./development/REFACTORING.md) – Refactoring criteria and procedures.
- [TECHNICAL_DEBT.md](./testing/TECHNICAL_DEBT.md) – Known technical debt and pending improvements.
- [KNOWN_ISSUES.md](./testing/KNOWN_ISSUES.md) – Known issues and limitations.
- [DEPRECATIONS.md](./testing/DEPRECATIONS.md) – Deprecated features and alternatives.
- [FLAKY_TESTS.md](./testing/FLAKY_TESTS.md) – Unreliable tests and corrective measures.
- [TEST_DATA.md](./testing/TEST_DATA.md) – Preparation, sourcing and management of test data.
- [COVERAGE.md](./testing/COVERAGE.md) – Objectives and interpretation of code coverage.
- [MUTATION_TESTING.md](./testing/MUTATION_TESTING.md) – Mutation testing methodology.

## 9. Security, privacy and compliance

- [SECURITY_POLICY.md](./security/SECURITY_POLICY.md) – Broader security policy.
- [THREAT_MODEL.md](./security/THREAT_MODEL.md) – Assets, threats, attack surfaces and mitigations.
- [SECURE_DEVELOPMENT.md](./security/SECURE_DEVELOPMENT.md) – Secure development practices.
- [SECURITY_ARCHITECTURE.md](./security/SECURITY_ARCHITECTURE.md) – Security controls and architecture.
- [VULNERABILITY_DISCLOSURE.md](./security/VULNERABILITY_DISCLOSURE.md) – Responsible disclosure procedure.
- [ACCESS_CONTROL.md](./security/ACCESS_CONTROL.md) – Roles, permissions and access rules.
- [ENCRYPTION.md](./security/ENCRYPTION.md) – Use of encryption and cryptographic decisions.
- [KEY_MANAGEMENT.md](./security/KEY_MANAGEMENT.md) – Key generation, custody, rotation and revocation.
- [SECRETS_MANAGEMENT.md](./security/SECRETS_MANAGEMENT.md) – Management of secrets and credentials.
- [PRIVACY.md](./privacy/PRIVACY.md) – Privacy considerations and data processing.
- [DATA_PROTECTION.md](./privacy/DATA_PROTECTION.md) – Data protection measures.
- [DATA_RETENTION.md](./privacy/DATA_RETENTION.md) – Data retention and deletion.
- [DATA_CLASSIFICATION.md](./security/DATA_CLASSIFICATION.md) – Classification of data by sensitivity.
- [COMPLIANCE.md](./compliance/COMPLIANCE.md) – Compliance requirements and applicable controls.
- [AUDIT.md](./security/AUDIT.md) – Scope or results of an audit.
- [SECURITY_AUDIT.md](./security/SECURITY_AUDIT.md) – Technical security audit.
- [PENTEST.md](./security/PENTEST.md) – Scope and methodology of a penetration test.
- [SBOM.md](./security/SBOM.md) – Explanation of the software component inventory.
- [SUPPLY_CHAIN_SECURITY.md](./security/SUPPLY_CHAIN_SECURITY.md) – Software supply chain risks.
- [DEPENDENCY_SECURITY.md](./security/DEPENDENCY_SECURITY.md) – Audit and management of vulnerable dependencies.
- [CRYPTOGRAPHY.md](./security/CRYPTOGRAPHY.md) – Cryptographic design and algorithms used.
- [ABUSE_CASES.md](./security/ABUSE_CASES.md) – Abuse cases and associated controls.
- [RISK_ASSESSMENT.md](./security/RISK_ASSESSMENT.md) – Risk identification and assessment.

## 10. User guides, tutorials and educational material

- [USER_GUIDE.md](./user-guide/USER_GUIDE.md) – Comprehensive user guide.
- [ADMIN_GUIDE.md](./guides/ADMIN_GUIDE.md) – Software operation and administration.
- [USAGE.md](./guides/USAGE.md) – Instructions for use and basic examples.
- [TUTORIAL.md](./tutorials/TUTORIAL.md) – Step-by-step practical tutorial.
- [TUTORIALS.md](./guides/TUTORIALS.md) – Index of tutorials.
- [EXAMPLES.md](./examples/EXAMPLES.md) – Usage examples.
- [COOKBOOK.md](./guides/COOKBOOK.md) – Recipes for common tasks.
- [CLI.md](./guides/CLI.md) – Using the command-line interface.
- [COMMANDS.md](./cli/COMMANDS.md) – Command reference.
- [GLOSSARY.md](./guides/GLOSSARY.md) – Definitions of terms.
- [LIMITATIONS.md](./guides/LIMITATIONS.md) – Unsupported features and known limitations.
- [MIGRATION_GUIDE.md](./migration/MIGRATION_GUIDE.md) – Detailed migration guide.
- [HOW_IT_WORKS.md](./guides/HOW_IT_WORKS.md) – Conceptual explanation of how it works.
- [CONCEPTS.md](./guides/CONCEPTS.md) – Fundamental concepts of the system.
- [RECIPES.md](./guides/RECIPES.md) – A collection of practical solutions.
- [BEST_PRACTICES.md](./guides/BEST_PRACTICES.md) – Best practices.
- [ANTI_PATTERNS.md](./guides/ANTI_PATTERNS.md) – Practices to avoid and the reasons why.
- [CHEATSHEET.md](./guides/CHEATSHEET.md) – Summary of commands or concepts for quick reference.
- [GLOSSARY_OF_TERMS.md](./guides/GLOSSARY_OF_TERMS.md) – Comprehensive technical glossary.
- [FAQ_DEVELOPERS.md](./development/FAQ_DEVELOPERS.md) – Frequently asked questions for developers.
- [FAQ_USERS.md](./user-guide/FAQ_USERS.md) – Frequently asked questions for users.
- [ACCESSIBILITY.md](./ACCESSIBILITY.md) – Accessibility guide or criteria for accessible use.
- `LOCALISATION.md` – How to add languages and translate the application.
- [TRANSLATION.md](./guides/TRANSLATION.md) – Translation workflow and string management.

## 11. Project management, planning and decision-making

- [PLAN.md](./project/PLAN.md) – Implementation or development plan.
- [TODO.md](./project/TODO.md) – Tasks to be done.
- [TASKS.md](./project/TASKS.md) – Task breakdown.
- [MILESTONES.md](./project/MILESTONES.md) – Milestones and verifiable objectives.
- [PROGRESS.md](./project/PROGRESS.md) – Progress tracking.
- [MEETING_NOTES.md](./meetings/MEETING_NOTES.md) – Meeting minutes or notes.
- [POSTMORTEM.md](./postmortems/POSTMORTEM.md) – Analysis of an incident or failure that has already occurred.
- [LESSONS_LEARNED.md](./project/LESSONS_LEARNED.md) – Lessons learnt from the project.
- [HANDOVER.md](./operations/HANDOVER.md) – Transfer of responsibilities or knowledge.
- [STAKEHOLDERS.md](./project/STAKEHOLDERS.md) – Stakeholders and their responsibilities.
- [PROJECT_CHARTER.md](./project/PROJECT_CHARTER.md) – Project objectives, scope, authority and framework.
- [RISK_REGISTER.md](./project/RISK_REGISTER.md) – Risk register, probability, impact and mitigation.
- [ASSUMPTIONS.md](./project/ASSUMPTIONS.md) – Planning assumptions and hypotheses.
- [SCOPE.md](./project/SCOPE.md) – Included and excluded scope.
- [CHANGE_REQUESTS.md](./project/CHANGE_REQUESTS.md) – Procedure for requesting and assessing changes.
- [DEFINITION_OF_DONE.md](./development/DEFINITION_OF_DONE.md) – Criteria for considering a task complete.
- [DEFINITION_OF_READY.md](./development/DEFINITION_OF_READY.md) – Criteria for considering a task ready.
- [WORKFLOW.md](./project/WORKFLOW.md) – General workflow for the team or project.
- [PROCESS.md](./project/PROCESS.md) – Operational or development process.
- [PRIORITIES.md](./project/PRIORITIES.md) – Criteria and order of priorities.
- [SUPPORT_MODEL.md](./operations/SUPPORT_MODEL.md) – Support model and responsibilities.

## 12. Versioning, release and compatibility

- [SEMANTIC_VERSIONING.md](./releases/SEMANTIC_VERSIONING.md) – How semantic versioning is applied.
- [RELEASE_PROCESS.md](./releases/RELEASE_PROCESS.md) – Complete release process.
- [RELEASE_CHECKLIST.md](./releases/RELEASE_CHECKLIST.md) – Pre-release checklist.
- [MIGRATION.md](./migration/MIGRATION.md) – Changes required when migrating.
- [BREAKING_CHANGES.md](./releases/BREAKING_CHANGES.md) – Breaking changes and their implications.
- [DEPRECATION_POLICY.md](./releases/DEPRECATION_POLICY.md) – Deprecation policy.
- [SUPPORT_POLICY.md](./releases/SUPPORT_POLICY.md) – Supported versions policy.
- [COMPATIBILITY_MATRIX.md](./releases/COMPATIBILITY_MATRIX.md) – Matrix of compatible versions, platforms or dependencies.
- [LIFECYCLE.md](./releases/LIFECYCLE.md) – Version or component lifecycle.
- [LTS.md](./releases/LTS.md) – Long-term support policy.
- [BACKPORTS.md](./releases/BACKPORTS.md) – Criteria for incorporating fixes into previous branches.
- [HOTFIX.md](./releases/HOTFIX.md) – Procedure for urgent fixes.
- [BRANCHING_STRATEGY.md](./development/BRANCHING_STRATEGY.md) – Git branching strategy.
- [TAGGING.md](./releases/TAGGING.md) – Conventions for Git tags.
- [CHANGE_MANAGEMENT.md](./releases/CHANGE_MANAGEMENT.md) – Change assessment, approval and control.

## 13. Infrastructure, networking and systems documentation

- [INFRASTRUCTURE.md](./infrastructure/INFRASTRUCTURE.md) – Infrastructure inventory and architecture.
- [INFRASTRUCTURE_OVERVIEW.md](./infrastructure/INFRASTRUCTURE_OVERVIEW.md) – Overview of resources and services.
- [NETWORK.md](./infrastructure/NETWORK.md) – Network design and operation.
- [NETWORKING.md](./infrastructure/NETWORKING.md) – Network and communications configuration.
- [DNS.md](./operations/DNS.md) – DNS configuration and name resolution.
- [TLS.md](./security/TLS.md) – TLS certificate configuration and renewal.
- [CERTIFICATES.md](./security/CERTIFICATES.md) – Certificate lifecycle management.
- [FIREWALL.md](./infrastructure/FIREWALL.md) – Firewall rules and design.
- [CONTAINERS.md](./infrastructure/CONTAINERS.md) – Container usage and architecture.
- [DOCKER.md](./infrastructure/DOCKER.md) – Building, running and configuring Docker.
- [KUBERNETES.md](./infrastructure/KUBERNETES.md) – Deployment and operation on Kubernetes.
- [HELM.md](./infrastructure/HELM.md) – Using Helm charts and configuration.
- [TERRAFORM.md](./infrastructure/TERRAFORM.md) – Organising and using Terraform.
- [INFRASTRUCTURE_AS_CODE.md](./infrastructure/INFRASTRUCTURE_AS_CODE.md) – Principles and workflow of infrastructure as code.
- [CLOUD_ARCHITECTURE.md](./architecture/CLOUD_ARCHITECTURE.md) – Cloud services architecture.
- [AWS.md](./infrastructure/AWS.md) – AWS-specific configuration or architecture.
- [AZURE.md](./infrastructure/AZURE.md) – Azure-specific configuration or architecture.
- [GCP.md](./infrastructure/GCP.md) – Google Cloud-specific configuration or architecture.
- [RESOURCE_LIMITS.md](./operations/RESOURCE_LIMITS.md) – Limits on CPU, memory, storage or other resources.
- [STORAGE.md](./infrastructure/STORAGE.md) – Storage design and operation.
- [HIGH_AVAILABILITY.md](./architecture/HIGH_AVAILABILITY.md) – Redundancy and fault tolerance.
- [NETWORK_SECURITY.md](./security/NETWORK_SECURITY.md) – Segmentation, network controls and risks.
- [ENVIRONMENT_TOPOLOGY.md](./infrastructure/ENVIRONMENT_TOPOLOGY.md) – Relationship between environments and their resources.

## 14. Data, databases and processing

- [DATABASE_SCHEMA.md](./data/DATABASE_SCHEMA.md) – Database schema.
- [MIGRATIONS.md](./data/MIGRATIONS.md) – Database migration management.
- [SEEDING.md](./data/SEEDING.md) – Initial data loading.
- [DATA_IMPORT.md](./data/DATA_IMPORT.md) – Data import.
- [DATA_EXPORT.md](./data/DATA_EXPORT.md) – Data export.
- [DATA_VALIDATION.md](./data/DATA_VALIDATION.md) – Data validation and integrity rules.
- [DATA_QUALITY.md](./data/DATA_QUALITY.md) – Data quality, consistency and completeness.
- [DATA_PIPELINE.md](./data/DATA_PIPELINE.md) – Processing and transformation flow.
- [ETL.md](./data/ETL.md) – Extraction, transformation and loading.
- [DATA_LINEAGE.md](./data/DATA_LINEAGE.md) – Data provenance and transformations.
- [DATA_DICTIONARY.md](./data/DATA_DICTIONARY.md) – Definition of fields, types and meanings.
- [DATA_GOVERNANCE.md](./data/DATA_GOVERNANCE.md) – Responsibilities, policies and data quality.
- [BACKUP_STRATEGY.md](./operations/BACKUP_STRATEGY.md) – Data backup and recovery strategy.
- [RETENTION_POLICY.md](./data/RETENTION_POLICY.md) – Data retention and disposal.
- [DATA_PRIVACY.md](./privacy/DATA_PRIVACY.md) – Privacy considerations in data processing.
- [ANALYTICS.md](./data/ANALYTICS.md) – Instrumentation, product metrics and analytics.
- [DATA_WAREHOUSE.md](./data/DATA_WAREHOUSE.md) – Data warehouse architecture.
- [STREAMING.md](./data/STREAMING.md) – Streaming data processing.
- [DATA_FORMATS.md](./data/DATA_FORMATS.md) – Supported data formats.

## 15. Documentation for AI tools and programming assistants

- [AGENTS.md](../AGENTS.md) – Instructions and context for supported programming agents.
- [CLAUDE.md](../CLAUDE.md) – Persistent instructions for Claude Code.
- [GEMINI.md](../GEMINI.md) – Context and instructions for Gemini CLI.
- [copilot-instructions.md](../.github/copilot-instructions.md) – General GitHub Copilot instructions for the repository.
- [project.instructions.md](../.github/instructions/project.instructions.md) – Copilot instructions with a specific scope based on your configuration (representative placeholder for the documented filename pattern).
- [SKILLS.md](./ai/SKILLS.md) — Catalogue of skills; none are currently published.
- [skills/NOTES.md](./ai/skills/NOTES.md) — Planned skills directory structure and conventions.
- [SKILL.md](./ai/templates/SKILL.md) — Template for creating an Agent Skill; not an active skill.
- [PROMPT.md](./ai/templates/PROMPT.md) – Template for a reusable prompt; not an active prompt.
- [PROMPTS.md](./ai/PROMPTS.md) – Catalogue of reusable prompts.
- [prompts/NOTES.md](./ai/prompts/NOTES.md) – Planned prompt directory structure and conventions.
- [AI_GUIDELINES.md](./ai/AI_GUIDELINES.md) – Guidelines for using AI in the project.
- [AI_POLICY.md](./ai/AI_POLICY.md) – AI usage policy.
- [CONTEXT.md](./ai/CONTEXT.md) – Context of an agent or automated process.
- [MODEL_CARD.md](./ai/MODEL_CARD.md) – Information about a model, its capabilities and limitations.
- [EVALUATION.md](./ai/EVALUATION.md) – Methodology for evaluating models or agents.
- [EVALS.md](./ai/EVALS.md) – Set or methodology of automated evaluations.
- [GUARDRAILS.md](./ai/GUARDRAILS.md) – Restrictions and controls for an AI system.
- [TOOLING.md](./development/TOOLING.md) – Tools available to the agent or team.
- [AGENT_ARCHITECTURE.md](./ai/AGENT_ARCHITECTURE.md) – Architecture of an agent or multi-agent system.

## 16. Site documentation, manuals and documentation generators

- [index.md](./index.md) – Home page for a documentation section.
- [mkdocs.yml](../mkdocs.yml) – MkDocs site configuration.
- [DOCS.md](./documentation/DOCS.md) – Table of contents or overview of the available documentation.
- [DOCUMENTATION.md](./documentation/DOCUMENTATION.md) – General guide to the project’s documentation.
- [DOCUMENTATION_GUIDE.md](./documentation/DOCUMENTATION_GUIDE.md) – Guidelines for writing and maintaining documentation.
- [WRITING_GUIDE.md](./documentation/WRITING_GUIDE.md) – Technical writing guidelines.
- [INFORMATION_ARCHITECTURE.md](./documentation/INFORMATION_ARCHITECTURE.md) – Organisation of information and navigation.
- [DOCS_ARCHITECTURE.md](./documentation/DOCS_ARCHITECTURE.md) – Internal organisation of the documentation system.
- [VERSIONED_DOCS.md](./documentation/VERSIONED_DOCS.md) – Version management for documentation.
- [TRANSLATION_GUIDE.md](./documentation/TRANSLATION_GUIDE.md) – Document translation process.
- [DOCS_DEPLOYMENT.md](./operations/DOCS_DEPLOYMENT.md) – Publication of the documentation site.
- [DOCS_MAINTENANCE.md](./documentation/DOCS_MAINTENANCE.md) – Documentation maintenance and review.

## 17. Legal documentation, licences and policies

- [TERMS.md](./legal/TERMS.md) – Terms of use.
- [TERMS_OF_SERVICE.md](./legal/TERMS_OF_SERVICE.md) – Terms of service.
- [PRIVACY_POLICY.md](./legal/PRIVACY_POLICY.md) – Privacy policy.
- [COOKIE_POLICY.md](./legal/COOKIE_POLICY.md) – Cookie policy.
- [ACCEPTABLE_USE_POLICY.md](./policies/ACCEPTABLE_USE_POLICY.md) – Permitted and prohibited uses.
- [DATA_PROCESSING.md](./privacy/DATA_PROCESSING.md) – Processing of personal data.
- [DATA_PROCESSING_AGREEMENT.md](./legal/DATA_PROCESSING_AGREEMENT.md) – Terms and conditions governing data processing between parties.
- [THIRD_PARTY_NOTICES.md](./legal/THIRD_PARTY_NOTICES.md) – Third-party attributions and notices.
- [EXPORT_CONTROL.md](./legal/EXPORT_CONTROL.md) – Export control considerations.
- [ETHICS.md](./policies/ETHICS.md) – Ethical principles of the project.
- [ACCESSIBILITY_POLICY.md](./policies/ACCESSIBILITY_POLICY.md) – Accessibility policy.

## 18. Scientific research, reproducibility and academic documentation

- [RESEARCH.md](./research/RESEARCH.md) – Research context and research questions.
- [METHODOLOGY.md](./research/METHODOLOGY.md) – Methodology used.
- [EXPERIMENTS.md](./research/EXPERIMENTS.md) – Design and record of experiments.
- [REPRODUCIBILITY.md](./research/REPRODUCIBILITY.md) – How to reproduce results or experiments.
- [DATASET.md](./data/DATASET.md) – Description of a dataset.
- [DATASET_CARD.md](./data/DATASET_CARD.md) – Origin, composition, limitations and uses of a dataset.
- [EXPERIMENT_LOG.md](./research/EXPERIMENT_LOG.md) – Record of experiments.
- [RESULTS.md](./research/RESULTS.md) – Results obtained and their interpretation.
- [ETHICS_STATEMENT.md](./research/ETHICS_STATEMENT.md) – Ethical considerations of a research project.
- [RESEARCH_QUESTIONS.md](./research/RESEARCH_QUESTIONS.md) – Research questions and hypotheses.
- [BIBLIOGRAPHY.md](./research/BIBLIOGRAPHY.md) – Bibliography in human-readable format.
- [REFERENCES.md](./research/REFERENCES.md) – References and sources.
- [REPLICATION_GUIDE.md](./research/REPLICATION_GUIDE.md) – Instructions for replicating a study.

## 19. Product, user experience and accessibility

- [PRODUCT.md](./product/PRODUCT.md) – Product vision and purpose.
- [PRODUCT_REQUIREMENTS.md](./product/PRODUCT_REQUIREMENTS.md) – Product requirements.
- [PRD.md](./product/PRD.md) – Product Requirements Document.
- [USER_STORIES.md](./product/USER_STORIES.md) – User stories and requirements.
- [PERSONAS.md](./product/PERSONAS.md) – Target user profiles.
- [USER_FLOWS.md](./design/USER_FLOWS.md) – User flows.
- [UX.md](./design/UX.md) – User experience guidelines.
- [UI.md](./design/UI.md) – Interface design and implementation.
- [BRANDING.md](./design/BRANDING.md) – Visual identity, tone and brand usage.
- [CONTENT_GUIDELINES.md](./product/CONTENT_GUIDELINES.md) – Content and microcopy guidelines.
- [EXPERIMENTATION.md](./product/EXPERIMENTATION.md) – A/B testing and product experiments.
- [FEATURE_FLAGS.md](./operations/FEATURE_FLAGS.md) – Use and management of toggleable features.
- [FEEDBACK.md](./product/FEEDBACK.md) – Channels and process for collecting feedback.
- [USER_RESEARCH.md](./research/USER_RESEARCH.md) – Methodology and results of user research.
- [INTERNATIONALIZATION.md](./product/INTERNATIONALIZATION.md) – Architecture and process for internationalisation.

## 20. Domain-specific documentation

- [BLOCKCHAIN.md](./architecture/BLOCKCHAIN.md) – Architecture and integration with blockchain.
- [SMART_CONTRACTS.md](./contracts/SMART_CONTRACTS.md) – Organisation, interfaces and behaviour of smart contracts.
- [TOKENOMICS.md](./domain/TOKENOMICS.md) – Economic design of tokens.
- [CONSENSUS.md](./architecture/CONSENSUS.md) – Consensus algorithm or mechanism.
- [WALLETS.md](./domain/WALLETS.md) – Wallet management and integration.
- [RPC.md](./domain/RPC.md) – RPC interfaces and node configuration.
- [NODE_OPERATIONS.md](./operations/NODE_OPERATIONS.md) – Installation, maintenance and operation of nodes.
- [MINING.md](./domain/MINING.md) – Mining design and operation, where applicable.
- [VALIDATORS.md](./domain/VALIDATORS.md) – Validator operation and responsibilities.
- [DEFI.md](./domain/DEFI.md) – Architecture of decentralised finance applications.

## Existing GitHub and documentation configuration

- [sidebars.js](../sidebars.js) – Configuration of the side navigation in Docusaurus.

- [docusaurus.config.js](../docusaurus.config.js) – Configuration for a Docusaurus documentation site.
- [config.yml](../.github/ISSUE_TEMPLATE/config.yml) – GitHub issue template selector and contact links.
- [bug_report.yml](../.github/ISSUE_TEMPLATE/bug_report.yml) – Structured bug reports.
- [feature_request.yml](../.github/ISSUE_TEMPLATE/feature_request.yml) – Structured feature proposals.
- [ideas.yml](../.github/DISCUSSION_TEMPLATE/ideas.yml) – Template for discussions about ideas.
- [q-a.yml](../.github/DISCUSSION_TEMPLATE/q-a.yml) – Template for questions and answers.
- [VULNERABILITY_REPORT.yml](../.github/VULNERABILITY_REPORT.yml) – Existing placeholder for vulnerability-reporting configuration.
- [FUNDING.yml](../.github/FUNDING.yml) – Sponsor and funding links.
- [CODEOWNERS](./CODEOWNERS) – Operational repository-wide code ownership rules (preferred location: `docs/`; GitHub lookup precedence differs).
