---
title: "aichat is transformative"
date: 2024-05-31
tags: [developer,sql,ai,llm]
type: blog
---
# aichat is a transformative find!

[aichat](https://github.com/sigoden/aichat) is a cli powered chat and copilot tool. Here is why I believe this statement:

I spend my day in the terminal writing code and takeing notes. Below is a phenomenal scenario that I believe any software development team could benefit from.

In my git repo, I have an aichat directory. It contains two types of files:

a. common repo prompts that many on the team would use (begins with 'prompt%') and
b. a specific task (begins with a datestamp) that I want an llm to help me with. 

Below is how I compose a prompt with little effort

```bash
aichat -f aichat/20240521-admin-introduction.txt \
       -f aichat/prompt-general.txt \
       -f migration-01-ddl.sql \
        > work-instruction-admin.txt
```

Where:

- 20240521-admin-introduction.txt is a file with text that includes the specific task to be completed (created by me - the one with the challenge to be solved)
- prompt-general.txt is a file that introduces the project core tenets (typically created by a team lead)
- [migration-01-ddl.sql](https://github.com/chuckstack/pg-workflow/blob/main/migration-01-ddl.sql) is the database design in its entirety (almost 30 tables) - notice the detailed table comments...
- Output: text file used for shared understanding (and that I might pass back into aichat if needed)

The quality of the resulting work instructions is crazy good. More specifically, the llm's ability to build a mental model and reason about the domain just from the sql ddl is hard to believe. By adopting a standard approach to how to engage an llm, the team shares in the ability to create better results. Aichat helps the team build the intelligence directly into the git repository without any dependency on any other locally installed tool.

Here is an example aichat directory:
```bash
❯ tree
.
├── 20240521-admin-introduction.txt
├── 20240521-mermaid-test.txt
├── 20240521-migration-config.txt
├── 20240521-not-null.txt
├── 20240521-plpgsql-api.txt
├── 20240522-admin-instruction.txt
├── 20240522-validate-best-practices-01.txt
├── 20240522-validate-best-practices.txt
├── 20240523-best-way-to-create-request-01.txt
├── 20240523-example-sql-01.txt
├── out
│   ├── 20240521-plpgsql-api.txt
│   ├── 20240523-best-way-to-create-request-01-01.out
│   ├── 20240523-best-way-to-create-request-01.out
│   ├── 20240523-example-sql-01.out
│   └── readme.md
├── prompt-coder.txt
├── prompt-example.txt
├── prompt-general.txt
├── prompt-migration-sql-change-instructions.txt
└── prompt-template.txt
```

More details if you are still reading:

- You can pipe one response to another request (each using a different model).
- You can create simple bash scripts to orchestrate higher level thinking like: ask once, ask again, ask yet again, ask for a final answer based on analyzing all previous responses.
- You can automate tasks around maintaining git repositories. for example: summarizing a file, using the file summaries to summarize a package, using package summaries summarize a repo. While these summaries might or might not help humans directly, these summaries can be piped into aichat (like above) to answer architectectural questions. For example: is what I am writing a 'pattern' or an 'anti-pattern' based on best practices.

The list goes on and on... I hope this helps!!

If you wish to learn more, join the [chuck-stack support academy](https://buy.stripe.com/7sIbLIeeU3oT4IEfYY).

Chuck Boecking
512.850.6068 (office and cell)
chuck@chuboe.com
www.ChuckBoecking.com
http://www.linkedin.com/pub/chuck-boecking/10/970/17b
