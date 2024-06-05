{
   "categories": "Программирование",
   "date": "2019-08-20",
   "tags": "Git",
   "title": "Очистить историю GIT"
}

```bash
git reset --soft $(git log --reverse --format=%H | head -n 1)
git commit --amend
git push -f
```

Только коллеги по проекту вам за это спасибо не скажут, имейте в виду...
