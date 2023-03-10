# Kubernetes Docs Lead Handbook
- [Overview](#overview)
    - [Common Terms](#common-terms)
- [Docs Lead Responsibilities](#docs-lead-responsibilities)
- [Prerequisites for Docs Lead and Shadows](#prerequisites-for-docs-lead-and-shadows)
    - [General Requirements](#general-requirements)
    - [Time Requirements](#time-requirements)
    - [Prerequisites for Docs Leads](#prerequisites-for-docs-leads)
    - [Prerequisites for Shadows](#prerequisites-for-shadows)
- [Release Timeline](#release-timeline)
- [Doc Authors and Contributors](#doc-authors-and-contributors)

## Overview

This document covers the responsibilities, time commitments, and timeline for Docs Leads shepherding docs releases for Kubernetes. Docs Lead Shadows should also read through this document and understand the launch processes so they can do it in the future.

### Common Terms

| Variable             | Explanation                                 | Example                                                  |
|----------------------|---------------------------------------------|----------------------------------------------------------|
| [current release]    | Active Kubernetes release                   | 1.13                                                     |
| [future release]     | Release that the team is actively composing | 1.14                                                     |
| [integration branch] | A PR [WIP] merging dev branch into main   | [link](https://github.com/kubernetes/website/pull/11401) |
|  ⚠️                   | Stresses extra importance                   |                                                          |

## Docs Lead Responsibilities

The Docs Lead is responsible for working with the Release Team to coordinate documentation updates for the next Kubernetes release.

Responsibilities include:

* Select and onboard Docs Lead Shadows to the release team
* Introduce and mentor Docs Lead Shadows regarding the release process and empowering them with the knowledge needed to be future Docs Leads
* Create an official Release Docs dev branch for the release and ensure it is [kept in sync throughout the release](https://github.com/kubernetes/sig-release/blob/master/release-team/role-handbooks/docs/Release-Timeline.md#maintain-the-current-and-upcoming-dev-branch)
* Identifying and tracking new Kubernetes features and feature updates that require new content
* Offering guidance to code contributors about where new feature and enhancements documentation should live
* Working with contributors to modify existing docs to accurately represent any upcoming changes
* Providing weekly updates to the Release Team about the current state of release-bound docs
* Reviewing documentation PRs to ensure quality following the website [Style Guide](https://kubernetes.io/docs/contribute/style/style-guide/)
* Migrating the old website [version] documentation and updating it with the new release
* Communicating changes with all of the localization branches in order to stay synced across repositories
* Updating these instructions with each release

* Understand the [Release timeline](https://github.com/kubernetes/sig-release/blob/master/release-team/role-handbooks/docs/Release-Timeline.md) and ensure that major Docs milestones are met according to schedule. The major milestones include: 
* Creating 
* Open placeholder PRs
* PRs ready for review
* All PRs reviewed and ready to merge

### Onboard the Release Lead Shadows
* Explain the responsibilities and expectations for the Docs Lead Shadow role, including the information available in the [Docs role handbook)[https://github.com/kubernetes/sig-release/tree/master/release-team/role-handbooks/docs], the [Release Timeline](https://github.com/kubernetes/sig-release/blob/master/release-team/role-handbooks/docs/Release-Timeline.md), and any other relevant sources. 
* Ask all shadows to open an issue against the kubernetes/org repo in order to become kubernetes/org member: [Issue: Organization Membership Request](https://github.com/kubernetes/org/issues/new?assignees=&labels=area%2Fgithub-membership&template=membership.yml&title=REQUEST%3A+New+membership+for+%3Cyour-GH-handle%3E). Shadows must mention sponsors on the issue. These sponsors should include the Docs Lead, Release Lead, and Emeritus Release Lead. 
* Create a PR to add the Docs Lead Shadows to the release-team.md file for the release (e.g. https://github.com/kubernetes/sig-release/blob/master/releases/release-1.27/release-team.md).
* Ensure the team has joined the [kubernetes-sig-release Google group](https://groups.google.com/g/kubernetes-sig-release).
* Ensure the release lead adds the team of Docs Lead Shadows to the [teams.yaml](https://github.com/kubernetes/org/blob/main/config/kubernetes/sig-release/teams.yaml) and verify all Docs Lead Shadows are included as members of the [release-team-docs](https://github.com/orgs/kubernetes/teams/release-team-docs/members). 
> Note: Docs Lead Shadows who are not members of this team will not be able to update the Enhancements Tracking Project created for the release. 

## Prerequisites for Docs Lead and Shadows

### General Requirements

Before continuing on to the Docs specific requirements listed below, please review and work through the tasks in the [Release Team Onboarding Guide](/release-team/release-team-onboarding.md).

### Time Requirements

A release is usually 12 weeks long. In general, there's a lot of work in the first few weeks of the release cycle to get the process started, and a lot of work in the last few weeks of the release cycle as documentation deadlines approach.

General time requirements for leads and shadows are:

- ½ hour to 2 hours a day, reviewing incoming enhancements, tracking documentation PRs, and monitoring Slack
- Between 1 and 2 hours a week to attend the majority of Release Team (weekly) and Burndown meetings (daily during Code Freeze), subject to time zone appropriateness
- Up to 1 hour weekly to attend [SIG Docs meetings](https://github.com/kubernetes/community/tree/master/sig-docs#meetings) for status reports

> Note: that the time commitment becomes greater closer to the release deadline, peaking during the final release day.

**During the last week of the release, shadows should expect to spend at least 5 hours and leads at least 10 hours finalizing the launch.**

### Prerequisites for Docs Leads

In addition to the time requirements above, a Docs Lead must:

- Have the ability to add a milestone to issues, so must be a member of the [website milestone maintainers](https://github.com/orgs/kubernetes/teams/website-milestone-maintainers/). Access can be requested by creating a [PR](https://github.com/kubernetes/org/pull/2235) against `kubernetes/org` repo.
> Note: access to see [website milestone maintainers](https://github.com/orgs/kubernetes/teams/website-milestone-maintainers/) is restricted to Kubernetes GitHub org members
- Have the ability to `/approve` PRs. Access can be requested by creating a [PR](https://github.com/kubernetes/website/pull/20351) against `main` branch.
- Take the [Inclusive Speaker Orientation (LFC101)](https://training.linuxfoundation.org/training/inclusive-speaker-orientation/) training course

### Prerequisites for Shadows

Docs Lead Shadows are people who are preparing to be a Docs Lead in the future. In addition to the time requirements above, shadows must:

- Have signed the [contributor CLA](https://github.com/kubernetes/community/blob/master/CLA.md) for Kubernetes.
- Be invested in becoming an org member within the release cycle. This can often be achieved during the release cycle with sponsorship from a role lead. See the [Release Team onboarding guide](/release-team/release-team-onboarding.md) for more details.
- General knowledge of our SIG-Docs [areas of responsibility](https://github.com/kubernetes/community/tree/master/sig-docs#subprojects).
- Experience with the general process involved with [contributing](https://kubernetes.io/docs/contribute/start/) to Kubernetes website.
- Have the ability to add a milestone to issues, so must be a member of the [milestone maintainers](https://github.com/orgs/kubernetes/teams/website-milestone-maintainers/). Access can be requested by creating a [PR](https://github.com/kubernetes/org/pull/2235) against `kubernetes/org` repo.

## Release Timeline

Reference the [release timeline documentation](Release-Timeline.md) for responsibilities during the release cycle.

## Doc Authors and Contributors

**Authors:** [Jim Angel](https://github.com/jimangel) & [Cody Clark](https://github.com/cody-clark)

Special thanks to contributors to this document, including:
* Andrew Chen
* Anna Jung
* Jared Bhatti
* Jennifer Rondeau
* Misty Linville
* Savitha Raghunathan
* Tim Bannister
* Tim Fogarty
* Zach Arnold
* Zach Corleissen

In addition, this document wouldn't be possible without the wonderful people in [#sig-docs](https://kubernetes.slack.com/messages/sig-docs)!
