# Ветвление, merge и rebase

## Что делали
Разыграли ситуацию, где команда правит один код: одну ветку влили через merge,
вторую — через rebase с разрешением конфликтов.

## merge
- Ветка `git-merge`: правки только в `merge.sh` (`$@`, затем вариант с `shift`).
- Влита в `main` мёрж-коммитом без конфликтов — правились разные файлы.

## rebase
- Ветка `git-rebase` ответвлена от базового коммита `prepare for merge and rebase`.
- `git rebase -i main` дал два конфликта в `rebase.sh` (оба разрешены вручную).
- После rebase — `push -f` (переписана история), затем merge в `main` перемоткой (fast-forward).

## Схема
https://github.com/IlyaSalih/devops_netology/network
