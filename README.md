# Export Github Project issues to CSV

Needed a simple way for non-developers to access issues in a Github Project.
Using the Github GraphQL API to fetch issues from a project in a private repo.

There are two different ways to display the data `table` or printed `csv`.
Nothing fancy, just an easy way to access data from the API to use in other software.

The fetched list contains the following data:

```
- Title
- Assignees
- Status (Custom Field)
- Milestone
- Development Area (Custom Field)
- Dev Estimate (Custom Field)
- Sprint (Custom Field)
```

## Config

There are just 4 variables to set:

```
const owner = "owner" // owner of the repo
const repo = "repo" // repo name
const projectId = 5 // project id
const token = "token" // personal access token, to access private repos/projects.
```

Necessary scopes for the access token:

```
 - repo
 - project
  - read:project
```

So this is just a single HTML-file with some inline CSS and JS.
