# Remote Repository Setup

## Current Remotes
```
backup	git@github.com:y8r1k/techstart-api-backup.git (fetch)
backup	git@github.com:y8r1k/techstart-api-backup.git (push)
origin	git@github.com:y8r1k/techstart-api.git (fetch)
origin	git@github.com:y8r1k/techstart-api.git (push)
```

## Tracking Branches
```
* main e7045ec [backup/main] Merge get_orders and get_info
```

## Fork Workflow Summary
- Original repository: [techstart-api](https://github.com/y8r1k/techstart-api)
- Fork repository: [techstart-api-backup](https://github.com/y8r1k/techstart-api-backup)
- Upstream configuration: `git remote add <remote>`

## Backup Strategy
- Primary remote: origin
- Backup remote: backup
- Sync command:
```
git fetch origin
git merge origin/main
git push backup main
```

## Lessons Learned
Довольно удобный инструмент ведения нескольких версий проекта, без необходимости хранить копии и помнить где какая. + История изменений
