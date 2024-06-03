# chuck-stack Introduction

## Purpose
The purpose of the chuck-stack is to help organizations: 
- increase transactional velocity and efficiency,
- identify and deploy AI-enabled, self-service tools that drive innovation from everyone in your organization,
- build a community of support and innovation.

## Why chuck-stack is Important
We believe in a cooperative approach to learning, support and innovation. As a group, we establish the priciples that guide decisions and collectively create a platform the values simplicity, stability and self-service.

## Target Organizations
We best support organizations that resemble the following characteristics:
- Generates between $10M and $500M in annual revenue or donations USD
- Supports multiple locations
- Has at least one person in IT
- Does not want to be locked into any one software (Microsoft) or platform (aws, gcp, azure) provider
- Needs a platform that leverages the least number of tools possible to promote in-depth knowlege and productivity with the tools that are used
- Wants to deliver organization-wide self-service abilities where possible so that IT can focus on platform improvements and education (and not simply executing a backlog of support tickets)

## Our Goals for your Organization
- Minimize complexity by minimizing the number of IT-tools used by the organization
- Maximize productivity by maximizing IT's ability to provide self-service tools within the organization
- Remove the IT department as a blocker for strategic initiative execution
- Minimize infrastructure cost

## We Love Training and Support
If you want training and support for any of the below tools, join the transaction-academy. We meet 4 times per week via zoom to learn, audit, deploy, support and scale the below systems.

[Subscribe Now](https://buy.stripe.com/7sIbLIeeU3oT4IEfYY)

## chuck-stack Internal Tools
AI-enabled collection of PostgreSQL extensions to:
- pg_stack_workflow - workflow engine
- pg_stack_form - create html forms on demand
- pg_stack_chart - creates html charts on demand
- pg_stack_asi - attribute, attribute set, attribute set instance - used to assign metabase to any record
- pg_stack_timesheet - timesheet engine
- pg_stack_dms - document management system - uses pg_stack_asi
- pg_stack_changelog - changelog engine
- pg_stack_tag - record tagging system - uses pg_stack_asi

## AI Enabled Tooling
What are AI enabled extensions?
- Clearly defined work instructions and documentation that is easily digestible by off-the-shelf LLMs
- Simply written code and architectures so that AI easily understands and can reason about the domain
- Rag-ready content to ensure complete answers
- Additional fine-tuning to ensure fast and accurate answers
- Architecture where both the cli client as well as the database itself can query LLMs to support user operations

## chuck-stack External Tools
- [Linux](https://en.wikipedia.org/wiki/Linux) (compute) - best tool to run applications on just about any platform in the world.
- [NixOS](https://nixos.org/) (Linux OS) - specific distribution of Linux delivering the most control and compute options. Nix represents the easiest way to describe, deploy and maintain desktops and servers.
- [GitHub](https://github.com/) (code, information, collaboration) - best tool for managing information, instructions and discussions. It provides most options for AI amplification.
- [Incus](https://linuxcontainers.org/incus/docs/main/) (virtualization) - container and virtual machine (VM) tool to develop, test and deploy IT applications.
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
- [Nushell](https://www.nushell.sh/) - (system and data) Terminal shell with designed to understand and manipulate structured data.
- [Zellij](https://www.zellij.dev) - terminal workspace environment for managing information and transactions.

## Guidelines for chuck-stack Selection
The chuck-stack has been cultivated over the last 25 years. Here are the guidelines for inclusion.
- Open source - or at least as open as possible
- Start simple - easy to understand and reason about. Nix pushes this concept a little (or a lot); however, the power and simplicity it creates is worth the extra effort
- Basic functionality - supports basics like CRUD (create, read, update and delete) with minimal effort
- Kind educator - needs someone in the community who makes the technology kind to the target audience
- Kind integrator - needs someone local to you digitally to help you leverage the tool
- Synergy - supports other tools in the stack. Example: runs on or integrates with postgresql
- Simple architecture - not overly complicated relative to the tool's purpose
- Enterprise scalability - it needs to scale to support an organization of at lease 100 people if not 1000 across multiple continents
- Enterprise testing and deployment - it needs to support team development where improvements can be development, tested and accepted in dedicated environments and easily migrated to production using CI/CD concepts or scripts
- Command Line Interface (CLI) centric - we love cli interfaces because they are easy to administer from anywhere.
- REST centric - we love scriptable interfaces that can be called from anywhere.

## Tools that I am Considering/Testing
- [Lightdash](https://www.lightdash.com/) - cli, dbt and SQL first BI tool
  - [example](https://www.loom.com/share/c0805a236a994de397ac5142fdfe4b7f) showing how dbt + lightdash work together.
- [Supabase](https://supabase.com/) - hosted postgresql that promotes creating users in the database and using impersonation as a strategy to write access logic once in a single location.
- [Tailscale](https://tailscale.com/) - zero-trust networking and vpn solution to allow access to privately shared networks. Most organizations have an opinion regarding this topic. The questions is: can tailscale operate as a default options in the absence of opinion.
- [Deepnote](https://deepnote.com/) - jupyter notebook
- [Grafana](https://grafana.com/) - alternative to Zabbix - default used to monitor incus.
- [Mattermost](https://mattermost.com/) - alternative to github - collaboration/discussions tools similar to Slack that stores data directly in PostgreSQL.
- [Discourse](https://www.discourse.org/) - alternative to github for collaboration/discussions

## What is Missing
All the chuck-stack tools are general tools that most organizations would use. Here are some tools that are missing from the list:
- workflow - I have tried various tools over the years; however, I have not found any tools that meet the stack selection criteria. They have been too complicated to install, too complicated to learn and/or too complicated to maintain. My hope is to find a workflow engine that runs directly out of PostgreSQL that can be exposed through PostgREST.
