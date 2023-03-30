# Getting Started

Welcome to your new project.

It contains these folders and files, following our recommended project layout:

File or Folder | Purpose
---------|----------
`app/` | content for UI frontends goes here
`db/` | your domain models and data go here
`srv/` | your service models and code go here
`package.json` | project metadata and configuration
`readme.md` | this getting started guide


## Next Steps

- Open a new terminal and run `cds watch` 
- (in VS Code simply choose _**Terminal** > Run Task > cds watch_)
- Start adding content, for example, a [db/schema.cds](db/schema.cds).


## Learn More

Learn more at https://cap.cloud.sap/docs/get-started/.
# cap-project-structure



# Bash - Terminal

user: projects $ cds init shop-manager
Creating new cap project in ./shop-manager

Adding feature 'nodejs'... 
Done adding features

Continue with 'cd shop-manager'
Find samples on https://github.com/SAP-samples/cloud-cap-samples
Learn about next steps at https://cap.cloud.sap

user: projects $ cd shop-manager/
user: shop-manager $ cds add samples
Adding feature(s) to project in current folder

Adding feature 'samples'... 
Done adding features


user: shop-manager $ cds watch
 
cds serve all --with-mocks --in-memory? 
watching: cds,csn,csv,ts,mjs,cjs,js,json,properties,edmx,xml,env,css,gif,html,jpg,png,svg... 
live reload enabled for browsers 

        ___________________________

 
[cds] - loaded model from 2 file(s):

  db/data-model.cds
  srv/cat-service.cds

[cds] - connect using bindings from: { registry: '~/.cds-services.json' }
[cds] - connect to db > sqlite { database: ':memory:' }
  > init from db/data/my.bookshop-Books.csv 
/> successfully deployed to in-memory database. 

[cds] - serving CatalogService { path: '/catalog' }

[cds] - server listening on { url: 'http://localhost:4004' }
[cds] - launched at 3/30/2023, 3:53:12 PM, version: 6.7.0, in: 1.519s
[cds] - [ terminate with ^C ]

[cds] - GET /catalog/Books 
^C
[cds] - my watch has ended.  
user: shop-manager $ ^C
user: shop-manager $ git init
Initialized empty Git repository in /home/user/projects/shop-manager/.git/
user: shop-manager $ git add -A
user: shop-manager $ git commit -m "inital project structure with sample data"
[main (root-commit) bc4292a] inital project structure with sample data
 10 files changed, 178 insertions(+)
 create mode 100644 .cdsrc.json
 create mode 100644 .gitignore
 create mode 100644 .vscode/extensions.json
 create mode 100644 .vscode/launch.json
 create mode 100644 .vscode/tasks.json
 create mode 100644 README.md
 create mode 100644 db/data-model.cds
 create mode 100644 db/data/my.bookshop-Books.csv
 create mode 100644 package.json
 create mode 100644 srv/cat-service.cds
user: shop-manager ^C        
user: shop-manager $ git remote add origin https://github.com/SheshnathA/cap-project-structure.git
user: shop-manager $ git branch
* main
user: shop-manager $ git pull https://github.com/SheshnathA/cap-project-structure.git main
From https://github.com/SheshnathA/cap-project-structure
 * branch            main       -> FETCH_HEAD
fatal: refusing to merge unrelated histories
user: shop-manager $ git pull origin main  --allow-unrelated-histories
From https://github.com/SheshnathA/cap-project-structure
 * branch            main       -> FETCH_HEAD
CONFLICT (add/add): Merge conflict in README.md
Auto-merging README.md
Automatic merge failed; fix conflicts and then commit the result.
user: shop-manager $ git status
On branch main
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both added:      README.md

no changes added to commit (use "git add" and/or "git commit -a")
user: shop-manager $ git add .
user: shop-manager $ git commit -m "inital project structure witrh samples data for service"
[main 952a536] inital project structure witrh samples data for service
user: shop-manager $ git push origin main
Enumerating objects: 21, done.
Counting objects: 100% (21/21), done.
Delta compression using up to 8 threads
Compressing objects: 100% (16/16), done.
Writing objects: 100% (19/19), 3.12 KiB | 1.56 MiB/s, done.
Total 19 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), done.
To https://github.com/SheshnathA/cap-project-structure.git
   8a9a147..952a536  main -> main