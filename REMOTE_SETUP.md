# Remote Repository Setup

## Current Remotes
backup	git@github.com:Zhitkov-Maks/techstart-api-backup.git (fetch)
backup	git@github.com:Zhitkov-Maks/techstart-api-backup.git (push)
origin	git@github.com:Zhitkov-Maks/techstart-api.git (fetch)
origin	git@github.com:Zhitkov-Maks/techstart-api.git (push)
origin	git@github.com:Zhitkov-Maks/techstart-api-backup.git (push)


## Tracking Branches
  develop 2c166f7 [origin/develop] changed version
* main    1da8147 [origin/main] Merge branch 'main' of github.com:Zhitkov-Maks/techstart-api


## Fork Workflow Summary
- Original repository: https://github.com/Zhitkov-Maks/awesome-calculator
- Fork repository: https://github.com/mzhitkov04-sys/awesome-calculator
- Upstream configuration: git remote add upstream git@github.com:mzhitkov04-sys/awesome-calculator.git

## Backup Strategy
- Primary remote: https://github.com/Zhitkov-Maks/techstart-api.git
- Backup remote: https://github.com/Zhitkov-Maks/techstart-api-backup.git
- Sync command: git push --all origin && git push --all backup

## Lessons Learned
Настройка upstream связей упрощает работу - можно использовать просто `git push` вместо `git push origin branch-name`. Remote-tracking ветки показывают состояние удаленных репозиториев без переключения между ветками. Резервные копии через несколько remote защищают от потери кода.
