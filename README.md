# Chuck-Stack Introduction

## Purpose
The purpose of the Chuck-Stack is to provide organizations with a technology stack and resources that maximize productivity and minimize cost. Deliver AI-enabled, self-help tools supporting innovation and efficiencies from anyone at any level.

Target Organization:
- Generates between $10M and $500M in annual revenue USD
- Has at least one person in IT
- Does not want to be locked into any one software (Microsoft) or platform provider (aws, gcp, azure)
- Needs a platform that leverages the least number of tools possible to promote in-depth knowlege and productivity with the tools that are used
- Wants to delivery self-serve abilities where possible so that IT can focus on platform evaluation and education (and not simply executing a backlog of support tickets)

## Goals
- Minimize complexity by minimizing the number of IT-tools used by the organization
- Maximize productivity by maximizing IT's ability to provide self-help tools within the organization
- Remove the IT department as a blocker for strategic initiative execution
- Minimize infrastructure cost

To support this project and its teaching efforts ...

To learn more about the Chuck-Stack organization, see our website ...

## Chuck-Stack
- [GitHub](https://github.com/) (code, information, collaboration) - best tool for managing "information". It provides most options for AI amplification.
- [NixOS](https://nixos.org/) (OS) - create operating systems (OS) for application delivery to anywhere from desktops to servers to tablets. Easiest way to describe and deploy and maintain the right OS tools to the right role.
- [Incus](https://linuxcontainers.org/incus/docs/main/) (virtualization) - container and VM tool to enable sub-organizations to innovate and deploy applications. Best virtualization tool that starts simple and scales to enterprise levels.
- [PostgreSQL](https://www.postgresql.org/) (data) - best tool for managing "data" - database with best performance and enterprise features.
- [PostgREST](https://postgrest.org/) (API) - PostgreSQL tool for exposing an OpenAPI compliant REST interface directly out of your database.
- [dbt](https://www.getdbt.com/) (ETL) - tool to transform transactional data into a form than can be consumed by BI or AI or ...
- [PostgresML](https://postgresml.org/) (AI) - PostgreSQL tool for AI training and inferencing directly out of your database.
- [Ollama](https://ollama.com/) (AI) - AI tool for running generative AI (LLM) models locally.
- [LangChain](https://www.langchain.com/) (AI) - high-level Python framework for programmatically interacting with AI (LLM) models.
- [Metabase](https://www.metabase.com/) (BI) - BI tool for visualizing and publishing data. Used if GitHub discussions is not good enough.
- [iDempiere](https://www.idempiere.org/) (ERP) - ERP for managing orders, inventory, invoices, payments, accounting and much of the data you need to execute operations in your organization.
- [Neovim](https://neovim.io/) (text editor, information) - Extremely powerful text editor. This tool is the most controversial because it is the least "simple" to get started. The fact that is can run in any terminal in almost any OS from almost any location overcomes that lack of initial simplicity.
- [Pass](https://passwordstore.org) - (secrets) - simply yet powerful password tool with clients for every major platform.
- [Zabbix](https://www.zabbix.com/) - (monitoring) monitor resources and respond to events.
- [CrowdSec](https://www.crowdsec.net/) - (security) Proactively block known malicious IPs and activities.

## Guidelines for Stack Selection
The Chuck-Stack has been cultivated over the last 25 years. Here are the guidelines for inclusion.
- Open source - or at least as open as possible
- Start simple - easy to understand and reason about. Nix pushes this concept a little (or a lot); however, the power and simplicity it creates is worth the extra effort
- Basic functionality - supports basics like CRUD (create, read, update and delete) with minimal effort
- Kind educator - needs someone in the tools who makes the technology kind to the target audience
- Kind integrator - needs someone local to you digitally to help you leverage the tool
- Synergy - supports other tools in the stack. Example: runs on or integrates with postgresql
- Simple architecture - not overly complicated given the tool's domain
- Enterprise scalability - it needs to scale to support an organization of at lease 100 people if not 1000 across multiple continents
- Enterprise testing and deployment - it needs to support team development where improvements can be development, tested and accepted in dedicated environments and easily migrated to production using CI/CD concepts or scripts

## Why the Stack is Important
- Principled (see guidelines)
- Protection against vendor-lock-in

## Tools that I am Considering
- [Lightdash](https://www.lightdash.com/) - cli, dbt and SQL first BI tool
  - [example](https://www.loom.com/share/c0805a236a994de397ac5142fdfe4b7f) showing how dbt + lightdash work together.
- [Supabase](https://supabase.com/) - hosted postgresql that promotes creating users in the database
- [Deepnote](https://deepnote.com/) - jupyter notebook
- [Grafana](https://grafana.com/) - alternative to Zabbix - default used to monitor incus.
- [Mattermost](https://mattermost.com/) - alternative to github - collaboration/discussions tools similar to Slack that stores data directly in PostgreSQL.
- [Discourse](https://www.discourse.org/) - alternative to github for collaboration/discussions

## What is Missing
All the Chuck-Stack tools are general tools that most organizations would use. Here are some tools that are missing from the list:
- workflow - I have tried various tools over the years; however, I have not found any tools that meet the stack selection criteria. They have been too complicated to install, too complicated to learn and/or too complicated to maintain. My hope is to find a workflow engine that runs directly out of PostgreSQL that can be exposed through PostgREST.
