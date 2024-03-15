# ChuckStack Introduction

## Purpose
The purpose of the ChuckStack is to provide organizations with a technology stack that maximizes productivity. It's optimized for the AI world where innovation and efficiencies can come from anyone at any level.

To support this project and its teaching efforts ...

To learn more about the ChuckStack organization, see our website ...

## ChuckStack
- [GitHub](https://github.com/) (code, information, collaboration) - best tool for managing "information". It provides most options for AI amplification.
- [NixOS](https://nixos.org/) (OS) - create operating systems (OS) for application delivery to anywhere from desktops to servers to tablets. Easiest way to describe and deploy and maintain the right OS tools to the right role.
- [Incus](https://linuxcontainers.org/incus/docs/main/) (virtualization) - container and VM tool to enable sub-organizations to innovate and deploy applications. Best virtualization tool that starts simple and scales to enterprise levels.
- [PostgreSQL](https://www.postgresql.org/) (data) - best tool for managing "data" - database with best performance and enterprise features.
- [PostgREST](https://postgrest.org/) (API) - PostgreSQL tool for exposing an OpenAPI compliant REST interface directly out of your database.
- [PostgresML](https://postgresml.org/) (AI) - PostgreSQL tool for AI training and inferencing directly out of your database.
- [Ollama](https://ollama.com/) (AI) - AI tool for running generative AI (LLM) models locally.
- [LangChain](https://www.langchain.com/) (AI) - high-level Python framework for programmatically interacting with AI (LLM) models.
- [Metabase](https://www.metabase.com/) (BI) - BI tool for visualizing and publishing data.
- [Mattermost](https://mattermost.com/) (collaboration) - collaboration tools similar to Slack that stores data directly in PostgreSQL.
- [iDempiere](https://www.idempiere.org/) (ERP) - ERP for managing orders, inventory, invoices, payments, accounting and much of the data you need to execute operations in your organization.
- [Neovim](https://neovim.io/) (text editor, information) - Extremely powerful text editor. This tool is the most controversial because it is the least "simple" to get started. The fact that is can run in any terminal in almost any OS from almost any location overcomes that lack of initial simplicity.

## Guidelines for Stack Selection
The ChuckStack has been cultivated over the last 25 years. Here are the guidelines for inclusion.
- Open source - or at least as open as possible
- Start simple - easy to understand and reason about
- Basic functionality - supports basics like CRUD (create, read, update and delete) with minimal effort
- Kind educator - needs someone in the tools who makes the technology kind to the target audience
- Kind integrator - needs someone local to you digitally to help you leverage the tool
- Simple - not overly complicated
- Enterprise scalability - it needs to be more than a toy
- Enterprise testing and deployment - it needs to support team development where improvements can be development, tested and accepted in dedicated environments

## Why the Stack is Important
- Principled (see guidelines)
- Protection against vendor-lock-in

## Tools that I am Considering
- [Deepnote](https://deepnote.com/)

## What is Missing
All the ChuckStack tools are general tools that most organizations would use. Here are some tools that are missing from the list:
- workflow - I have tried various tools over the years; however, I have not found any tools that meet the stack selection criteria. They have been too complicated to install, too complicated to learn and/or too complicated to maintain. My hope is to find a workflow engine that runs directly out of PostgreSQL that can be exposed through PostgREST.
