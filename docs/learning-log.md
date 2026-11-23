# Learning Log

## 2026-11-22, Repo setup
- Did: created the repo, structure, README and roadmap
- Learned: Git doesn't track empty folders, so we use .gitkeep
- Unclear: (none yet)

## 2026-11-23, Session 1: Docker basics (in progress)
- Did: ran nginx and Postgres containers, used run, ps, logs, exec, rm
- Broke: reused the name "web" (name already in use), then reused port 8081 (port is already allocated)
- Learned: a failed docker run can leave a container in Created state; a typo of /q instead of \q left psql waiting at postgres-#
- Confirmed: without a volume, the table was gone after removing the container
- Next: repeat with -v pgdata and confirm the table survives
- Parking lot: how do volumes actually work on disk?