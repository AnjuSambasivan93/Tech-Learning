
# Jira Notes

## What is Jira?

Jira is an issue-tracking and project management tool developed by Atlassian. It is mainly used by software development teams to plan work, manage tasks, track bugs, and monitor project progress.

Jira supports Agile methodologies such as Scrum and Kanban.

## Key Concepts

### Project
A collection of related work, such as developing a web application.

### Issue (Work Item)
An individual piece of work tracked in Jira.

Common issue types:
- **Bug:** A problem that needs fixing.
- **Task:** General work that needs completing.
- **Story:** A feature or requirement from a user's perspective.
- **Epic:** A large feature divided into smaller stories or tasks.
- **Subtask:** A smaller part of a task.

### Backlog
A prioritised list of work that has not yet been completed or scheduled.

### Sprint
A fixed period of development in Scrum, usually 1–4 weeks, during which the team works toward a Sprint Goal.

### Workflow
The sequence of statuses through which an issue progresses.

Typical workflow:

`To Do → In Progress → Code Review → Testing → Done`

Workflows can vary between projects.

## Jira Issue Fields

Each issue can contain:

- **Issue Key:** Unique identifier, e.g. `PROJ-101`.
- **Summary:** Short description of the work.
- **Description:** Detailed requirements or problem.
- **Assignee:** Person responsible.
- **Reporter:** Person who created or reported the issue.
- **Priority:** Importance or urgency.
- **Status:** Current stage of work.
- **Labels:** Tags used to categorise issues.
- **Comments:** Updates and discussions.
- **Attachments:** Screenshots, logs or documents.

## Jira Boards

A Jira board visually displays work using columns representing workflow stages.

### Scrum Board
Used by teams working in fixed-length Sprints.

Supports:
- Product Backlog
- Sprint Planning
- Sprint Backlog
- Sprint progress tracking
- Burndown charts

### Kanban Board
Used to manage a continuous flow of work.

Supports:
- Visualising tasks
- Tracking progress
- Limiting Work in Progress (WIP)
- Identifying bottlenecks

**Difference:** Scrum organises work into Sprints, while Kanban focuses on continuous flow.

## Agile in Jira

Agile is an iterative approach to software development that encourages collaboration, frequent feedback, and continuous improvement.

Jira helps teams apply Agile practices.

Common Scrum events:
- **Sprint Planning:** Decide what to work on during the Sprint.
- **Daily Scrum:** Inspect progress toward the Sprint Goal and adapt the plan.
- **Sprint Review:** Review the outcome with stakeholders.
- **Sprint Retrospective:** Identify improvements for future Sprints.

## Bug Tracking

Jira is commonly used to manage software defects.

A bug report should include:
- Description of the problem
- Steps to reproduce
- Expected result
- Actual result
- Environment (browser, operating system, application version)
- Severity or priority
- Screenshots or error logs when available

A developer investigates the issue, implements a fix, tests it, and updates the ticket.

## Jira and Git

Jira manages development work, while Git manages source code versions.

Jira can integrate with GitHub, GitLab, and other development tools.

Developers can:
- Link commits to Jira issues.
- Associate branches with work items.
- Link pull requests to issues.
- Track development progress.

Example Git branch:

`feature/PROJ-101-login-validation`

The issue key helps connect the code change with the Jira task.

## Jira Query Language (JQL)

JQL is used to search and filter Jira issues.

Examples:

Find open issues:

```jql
status = "To Do"
```

Find high-priority bugs:

```jql
issuetype = Bug AND priority = High
```

Find issues assigned to the current user:

```jql
assignee = currentUser()
```

Find issues in a project:

```jql
project = PROJ ORDER BY created DESC
```

## Jira Reports

Jira provides reports to monitor project progress.

- **Burndown Chart:** Shows remaining Sprint work over time.
- **Velocity Chart:** Shows work completed across Sprints.
- **Cumulative Flow Diagram:** Shows how work moves through workflow statuses.
- **Control Chart:** Helps analyse cycle time and process performance.

Report availability depends on project configuration.

## Benefits of Jira

- Centralised task and bug tracking
- Clear ownership and accountability
- Better team collaboration
- Visibility into project progress
- Support for Agile development
- Integration with development tools
- Documentation of issues and decisions

## Quick Summary

Jira is used to organise, assign, track, and manage software development work.

The most important concepts are:

**Projects, Issues, Bugs, Stories, Epics, Backlogs, Sprints, Workflows, Scrum, Kanban, and JQL.**

Official documentation: https://www.atlassian.com/software/jira/guides
