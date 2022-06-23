---
id: orientation
title: How to contribute to Polygon
description: We believe one of the things that makes Polygon special is its coherent design, and we seek to preserve this defining characteristic.
keywords:
  - docs
  - matic
image: https://matic.network/banners/matic-network-16x9.png 
---

## **Identifying an area to contribute**

There are several ways to identify an area where you can contribute to Polygon:

- The easiest is to simply send an email to one of our [Community Maintainers](/docs/contribute/community-maintainers) saying “I want to help!” They’ll work with you to find an area for you to contribute
- If you have a specific contribution in mind, first confirm whether this contribution is appropriate by reaching out in the Polygon Telegram group, or contacting one of our [Community Maintainers](/docs/contribute/community-maintainers) directly
- If you do not have a specific contribution in mind, you can browse the issues labelled as `help wanted` on the [Polygon GitHub repos](https://github.com/maticnetwork)
- Issues that also include the `good first issue` label are considered ideal for first-time contributors

## **Contribute to the Polygon Documentation:**
  - If you need to add or change anything in the Polygon Documentation, please raise a pull request (PR) to the `master` branch (kindly refer to the sample PR provided below)
  - The Polygon team will review the PR or reach out accordingly 
  - Repository: https://github.com/maticnetwork/matic-docs
  - Sample PR: https://github.com/maticnetwork/matic-docs/pull/360
  > If you are adding a new document, we recommended you provide a basic summary/introduction and a link to your github or documentation for more details

## **Contribution guidelines**

One of the things we believe makes Polygon special is its coherent design, and we seek to preserve this defining characteristic. From the outset, we defined some guidelines to ensure all new contributions always serve to enhance the project:

- **Quality**: All code in the Polygon project should meet the style guidelines. This means it must include sufficient test cases, descriptive commit messages, evidence that the contribution does not break any compatibility commitments or cause adverse feature interactions, and evidence of high-quality peer review
- **Size**: The Polygon project’s culture is one of small PRs, regularly submitted. The larger a PR, the more likely it is that you will be asked to resubmit in a series of self-contained and individually reviewable smaller PRs
- **Maintainability**: If the feature will require ongoing maintenance (e.g. support for a particular brand of database), we may ask you to accept responsibility for maintaining this feature

### Git Rules

We use `gitchangelog` for all of our repos for change logs. To do this, we apply a commit message convention. Merge requests that do not follow this convention will not be approved.

**Commit message convention**

The following are suggestions that might be useful to think about adding to your commit messages. You should consider separating your commits into broader categories:

- by intent (for example: new, fix, change ...)
- by object (for example: doc, packaging, code ...)
- by audience (for example: dev, tester, users ...)

Additionally, you may want to tag some commits:

- as “minor” commits that shouldn’t get output to your changelog (such as cosmetic changes, small typos in comments ...)
- as “refactor” if you don’t really have any significant feature changes. As such, this should not be part of the changelog displayed to the final user, but might be of interest if you have a developer changelog
- you could tag also with “api” for API changes, a new API or similar

Try writing your commit message by targeting user functionality as often as possible.

**Example**

This is a standard git log `--oneline` to show how the information could be stored:

```
* 5a39f73 fix: encoding issues with non-ascii chars.
* a60d77a new: pkg: added ``.travis.yml`` for automated tests. 
* 57129ba new: much greater performance on big repository by issuing only one shell command for all the commits. (fixes #7)
* 6b4b267 chg: dev: refactored out the formatting characters from GIT.
* 197b069 new: dev: reverse ``natural`` order to get reverse chronological order by default. !refactor 
* 6b891bc new: add utf-8 encoding declaration !minor 
```

For more information about changelogs, see [What Are Some Good Ways to Manage a Changelog Using Git?](https://stackoverflow.com/questions/3523534/good-ways-to-manage-a-changelog-using-git/23047890#23047890)

For more information about Git commit messages, see [https://chris.beams.io/posts/git-commit/](https://chris.beams.io/posts/git-commit/)
