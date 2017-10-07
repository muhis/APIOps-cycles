## Development Guidelines

This document intends to establish guidelines which build a transparent, open mechanism for deciding how to evolve the APIOps Cycles. 
The APIOps Developer Community will initially follow these processes when merging changes from external contributors or from the TDC itself. 
This guideline document will be adjusted as practicality dictates.

## APIOps Cycles Driving factors

The APIOps Cycles methodology should be use-case driven.  We can specify support for hypothetical use cases as we see fit, 
but methodologies should be backed by realistic scenarios.

## Methodologies Change Criteria

We should typically make changes when any of the following criteria are met:

 - Clarity.  The current "way" something is done doesn't make sense, is complicated, or not clear.
 - Consistency.  A portion of the methodology is not consistent with the rest
 - Necessary functionality.  We are missing functionality because of a certain design of the methodology.
 - Forward-looking designs.  As usage and business models of APIs evolves we should always consider what the next important aspect to consider and cover should be.
 - Impact.  A change will provide impact on a large number of use cases.  We should not be forced to accommodate every use case.  We should strive to make the _common_ and _important_ use 
 cases.  We cannot be edge-case driven.


## Tracking Process

 - Use GitHub for all methology designs, use cases, and so on.
 - At any given time, there would be _at most_ 2 work branches. The branches would exist if work has started on them. 
   - `master` - Current stable version. No PRs would be accepted directly to modify the methodology. PRs against supporting files can be accepted.
   - `development` - The next PATCH version of the specification. All changes to master will go through this version.  
 - The `master` branch shall remain the current, released APIOsp Cycles methodology.  
 - Examples of how something is described _currently_ vs. the proposed solution should accompany any change proposal.
 - New features should be done in feature branches/forks which, upon approval, are merged into the development branch.
 - Use labels for the workflow of specification changes.  Examples of labels are `proposed`, `needs migration review`, `needs tooling review`, `needs documentation`, `rejected`, and `needs approval`.  These labels must be assigned by project committers.
 - An issue will be opened for each feature change.  Embedded in the issue, or ideally linked in a file via pull-request (PR), a document about use cases should be supplied with the change.
 - A PR will be used to describe the _proposed_ solution, and linked to the original issue.
 - Not all committers will contribute to every single proposed change.  There may be many open proposals at once, and multiple efforts may happen in parallel.
 - When the a work branch is ready and approved, the branch will be merged to master.

## Approving Changes

For each change in the methodology we should _always_ consider the following:

 - Migration.  Is this a construct that has a path from the existing APIOps Cycles?  If so, how complicated is it to migrate to the proposed change?
 - Tooling.  Strive to support existing solutions in the markets. Are there practical tools to work with. These should be documented and considered during the change approval process.
 - Visualization.  Can the methodology change be graphically visualized somehow in a UI or other interface such as canvas?

Methodology changes should be approved by a majority of the committers.  
Approval can be given by commenting on the issue itself, for example, "Approved by @fehguy".  
After voting criteria is met, any committer can merge the PR. TODO: clarify voting 

No change should be approved until there is documentation for it, supplied in an accompanying PR.

## Transparency

We should always be as transparent as possible.  Sometimes there will be discussions that use customer names, sensitive use cases, and so on.  These must be anonymized, discussed in a private repository, or conducted offline.

 - Asynchronous discussions should live in the GitHub issues for this project.
 - Realtime discussions should be in a public Slack - apiops.slack.com.

