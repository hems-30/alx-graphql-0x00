# Episode Queries

This folder contains GraphQL queries and their outputs for retrieving specific episodes from the Rick and Morty GraphQL API.

## Files

| File | Description |
|------|-------------|
| `characters-page-1.graphql` | GraphQL query to fetch details of episode with ID 1 |
| `characters-page-1-output.json` | JSON output of episode 1 query |
| `characters-page-2.graphql` | GraphQL query to fetch details of episode with ID 2 |
| `characters-page-2-output.json` | JSON output of episode 2 query |
| `characters-page-3.graphql` | GraphQL query to fetch details of episode with ID 3 |
| `characters-page-3-output.json` | JSON output of episode 3 query |
| `characters-page-4.graphql` | GraphQL query to fetch details of episode with ID 4 |
| `characters-page-4-output.json` | JSON output of episode 4 query |

## Instructions

1. Each `.graphql` file contains a query using the `episode(id: ID!)` field to fetch:
   - `id`
   - `name`
   - `air_date`
   - `episode`

2. Each `.json` file is the output of its corresponding GraphQL query.

3. The queries can be run against the Rick and Morty API endpoint:  
   `https://rickandmortyapi.com/graphql`

4. Example query format (`characters-page-1.graphql`):

```graphql
query {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }