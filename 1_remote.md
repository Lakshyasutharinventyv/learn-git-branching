
### 1.1 Clone Intro
![image](https://github.com/user-attachments/assets/10373ef8-a56e-43a4-be0a-5e023818d475)
```sh
git clone <repository-url>
```

### 1.2 Remote Branches
![image](https://github.com/user-attachments/assets/5a7ce202-0a79-43fb-9044-24ee75cb1507)

```sh
git commit -m "Your commit message"
git checkout o/main
git commit -m "Another commit message"
```

### 1.3 Git Fetchin
![image](https://github.com/user-attachments/assets/de0d8217-ef03-460e-8be5-ea8be57bcde0)

```sh
git fetch
```

### 1.4 Git Pullin  
![image](https://github.com/user-attachments/assets/fc765721-2bc9-432c-99cc-125677e943b2)

```sh
git pull
```

### 1.5 Fakeing Teamwork 
![image](https://github.com/user-attachments/assets/9f614714-7476-4829-80b6-4625e9c9db2d)

```sh
git clone <repository-url>
git fakeTeamwork master 2
git commit -m "Simulated teamwork commit"
git pull
```

### 1.6 Git Pushin
![image](https://github.com/user-attachments/assets/dec847f8-f690-4b74-8a5c-78d26d5941c0)
 
```sh
git commit -m "First commit"
git commit -m "Second commit"
git push
```

### 1.7 Diverged History
Simulate teamwork, commit changes, and handle a diverged branch using rebase:  
```sh
git clone <repository-url>
git fakeTeamwork
git commit -m "Local commit"
git pull --rebase
git push
```

### 1.8 Locked branch Master  
Reset to the latest remote version and create a new feature branch:  
```sh
git reset --hard o/master
git checkout -b feature C2
git push
```

---

### 2.1 Push Master!
Rebase multiple branches onto `master` and push changes:  
```sh
git rebase side1 side2
git rebase side2 side3
git rebase side3 master
git pull --rebase
git push
```

### 2.2 Merging with remotes
Merge multiple branches into `main` and push the changes:  
```sh
git checkout main
git pull
git merge side1
git merge side2
git merge side3
git push
```

### 2.3 Remoting Tracking
Create a new branch tracking a remote branch and keep it updated:  
```sh
git checkout -b side o/main
git commit -m "New commit on side branch"
git pull --rebase
git push
```

### 2.4 Git push arguments 
Push specific branches to the remote repository:  
```sh
git push origin main
git push origin foo
```

### 2.5 Git push arguments — Expanded
Push commits from one branch to another:  
```sh
git push origin main~1:foo
git push origin foo:main
```

### 2.6 Fetch arguments 
Fetch commits and merge specific changes:  
```sh
git fetch origin main~1:foo
git fetch origin foo:main
git checkout foo
git merge c6
```

### 2.7 Source of nothing  
Delete remote branches by pushing an empty reference:  
```sh
git push origin :foo
git fetch origin :bar
```

### 2.8 Pull arguments 
Pull updates from one branch into another:  
```sh
git pull origin bar:foo
git pull origin main:side
```
