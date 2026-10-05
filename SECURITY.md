# Security Policy

## Supported versions

Only the latest commit on the default branch is supported. There are no maintained older releases.

## Reporting a vulnerability

Please **do not** open a public issue. Email **contact@examineip.com** with:

- the repository and file affected,
- what an attacker could do, and
- the smallest input that shows it.

You will get a reply as soon as possible. If the report is confirmed, a fix is published and you are
credited in the commit message unless you would rather not be.

## What counts

Anything that makes a library give a dangerously wrong answer counts as a security issue here, not
only code execution — for example, a blacklist check reporting a listed address as clean, an email
authentication check calling a forged message legitimate, or a lookalike-domain check missing a
disguised name.

The live tools on tools.examineip.com use these libraries; problems with the website itself can be
reported to the same address.
