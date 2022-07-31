# Pocketbase for Dokku

This repo can be used to deploy a new instance of pocketbase on dokku


## Dokku Workflow for creating a new instance of Pocketbase 

```bash
dokku apps:create pocketbase 

dokku domains:add pocketbase pocketbase.domain.name

dokku storage:mount pocketbase /var/lib/dokku/data/storage/pocketbase:/storage

dokku git:sync pocketbase https://github.com/kidGodzilla/pocketbase-dokku.git main --build
```
