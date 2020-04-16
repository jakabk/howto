#git
#branch
#delete
#local
#remote

# Delete git branches

## Local
> -d --delete, -D --delete --force

```bash
git branch --delete --force <branch-name>
```

## Remote
```bash
git push <remote-name, e.g. origin> --delete <branch-name>
```
> or
```bash
git push <remote-name, e.g. origin> :<branch-name>
```
