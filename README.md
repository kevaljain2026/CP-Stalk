# CPStalk

Data and Applications Monsoon 2022 Project

## Points

- Date is yyyy-mm-dd
  
## To Do

- Add Rank constraints based on rating or something
- Handle Ranks, you only need to update the ranks for a particular platform each time
- add table for user_team

## Commands

- create, update, delete cpstalk `user`
  - delete user wil automatically delete all cpstalk information related to the user, which is:
  - `friendship`, `submissions` (because we only store submissions related to cpstalk users), member from `team`
  
- create, update, delete username (`user_register_on`) for platform,
  - should modify platform users, how to decide `active users`?
  
- add, delete two users as `friends`

- create, modify, delete `team`

- create, modify, delete `contest`
  - add contest_id to `problem`?, value can be null
  
- create, modify, delete, problem `problem`, so including author, tags
  - add time of creation? so that time of submission is after creation?
  
- add submission to `practice`,
  - constraint, execution time and memory used < time limit and memory limit
- add submission to `attempts`,
  - constraint, execution time and memory used < time limit and memory limit
  - `attmepts_3` should only have `platform_name` and `submission_id` as primary key, then `teamID` could be null
- Also just add another table for `team_user`

- added ranks to `user_register_on`
- add, delete platform `language`??
  
## Constraints

- execution time of submission < time limit

## Modifications

- changed primary key to just `platform_name` and `submission_ID`, in `attempts_3` and `prac_3`

- created `team_users`, with attributes team_ID, username, platform:

- added `platform_name` to `problem_tags` and `problem_authors` as attributes and primary key

- add contest_id to problem? can be null;
  