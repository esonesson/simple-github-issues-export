# Export Github Project issues to CSV

Needed a simple way for non-developers to access issues in a Github Project.
Using the Github GraphQL API to fetch issues from a project in a private repo.

There are two different ways to display the data `table` or printed `csv`.
Nothing fancy, just an easy way to access data from the API to use in other software.

The fetched list contains the following data:

```
- Issue Number
- Title
- Assignees
- Status (Custom Field)
- Milestone
- Development Area (Custom Field)
- Current Estimate (Custom Field)
- Original Estimate (Custom Field)
- Sprint (Custom Field)
```

## Config

There is just 1 variables to set:

```
const token = "token" // personal access token, to access private repos/projects.
```

Necessary scopes for the access token:

```
 - repo
 - project
  - read:project
```

So this is just a single HTML-file with some inline CSS and JS. Neither pretty or optimized code, but it does the job as an internal tool.
