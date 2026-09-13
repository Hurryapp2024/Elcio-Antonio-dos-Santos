[← Back to portfolio](README.md)

# Track&Go
## Defining a connected workflow for field operations

**Focus:** Operations · Service coordination · Business requirements  
**Status:** Product in development. This is a design case, not a production performance report.

## The operational problem

Service businesses need to keep office planning aligned with work performed in the field. Scheduling changes, unclear assignments, and delayed completion updates make it harder to understand workload, service quality, and job-level costs.

Construction and cleaning operations informed the product direction.

## My contribution

I defined business use cases, mapped the relationship between scheduling and execution, and requested functionality that improves operational visibility. My role includes reviewing usability and refining priorities around daily work.

## Workflow design sample

The following sample organizes the product direction into a reviewable workflow. It describes intended behavior and does not certify that each step is implemented.

| Stage | Information needed | Responsible role | Intended handoff |
|---|---|---|---|
| Work intake | Customer, service, location, requested timing | Office | A clear work request |
| Planning | Estimated duration, availability, assigned team | Coordinator | An assigned visit or job |
| Execution | Instructions, current status, exceptions | Field team | A completion or exception update |
| Review | Completion details, unresolved issues, cost inputs | Supervisor / owner | Confirmation or follow-up |
| Financial follow-through | Agreed charge and relevant job costs | Office / owner | Information for billing and analysis |

## Design choices

**Connect planning with execution.** A schedule only creates operational visibility when field updates can be related to the planned work.

**Make exceptions visible.** Delays, access problems, and incomplete work need an explicit follow-up path.

**Keep financial context connected.** Operational activity should support a clearer understanding of the resources required for each job.

## Illustrative review scenario

A recurring cleaning visit requires reassignment. A reviewer should be able to determine:

1. Which visit changed and who owns the reassignment.
2. Whether the new team can access the relevant instructions.
3. Whether the office can distinguish scheduled, completed, and unresolved work.
4. Whether follow-up and cost information remain associated with the correct job.

This is a proposed acceptance scenario, not a reported test result.

## Measures to evaluate

| Proposed measure | What it would help assess |
|---|---|
| Assignment completeness | Whether scheduled work has a clear owner |
| Completion update timeliness | Whether the office receives useful field information |
| Rework frequency | Whether recurring service issues are visible |
| Availability of job-cost inputs | Whether operational records support financial review |

No measured baselines or improvements are presented. Evaluation requires a testable product and reliable operational data.

## What this work demonstrates

An ability to translate service-business experience into structured requirements, handoffs, and practical evaluation criteria.

[← Back to portfolio](README.md)
