# csg_proj

csg github demo using MERN stack

### Github documentation

https://docs.github.com/en/rest/reference/repos#list-repositories-for-a-user

#### TODOS

- backend:
  - resolve authentication errors when connecting to mongo atlas
  - setup calls to github endpoint
  - requery user info [FEATURE]
    - requery conditions:
      - scheduled jobs (see setInterval)
        - every x minutes, or at certain times in the day, hit github endpoint with current user and
          update db record
        - alternative: make calls to an endpoint that tells you only if a repo has been updated or not
      - when the user is inputted into the search form
- frontend:
  - active state management (global state libraries)
  - styling issues with margins
  - organize workflow to be less binary
    - single page workflow
  - add list of favorite users to regurlarly check github statuses [FEATURE]
    - available to organize user profiles like file directory in addition to favorites
- db:
  - create document for mongodb to store necessary information on our users
  - will need to coordinate with backend on requerying logic
    - possible to requery as little as needed?
      - tags, prs, equivalent of watching a repo
