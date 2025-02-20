### 2.1 Push Master!
![image](https://github.com/user-attachments/assets/3800ab54-3d49-4bcb-8fcc-3e8b920c058f)

```sh
git rebase side1 side2
git rebase side2 side3
git rebase side3 master
git pull --rebase
git push
```

### 2.2 Merging with remotes
![image](https://github.com/user-attachments/assets/6ebaf6fa-674f-48ad-a654-fd42f33a64ed)

```sh
git checkout main
git pull
git merge side1
git merge side2
git merge side3
git push
```

### 2.3 Remoting Tracking
![image](https://github.com/user-attachments/assets/e8a6584c-3375-43cf-8a80-9b8eb3f488d7)

```sh
git checkout -b side o/main
git commit
git pull --rebase
git push
```

### 2.4 Git push arguments 
![image](https://github.com/user-attachments/assets/ada88e72-a773-4b2c-9fe8-4971f5f6a86b)

```sh
git push origin main
git push origin foo
```

### 2.5 Git push arguments — Expanded
![image](https://github.com/user-attachments/assets/078e0fbf-7421-4f72-8a06-44b4fbb799aa)

```sh
git push origin main~1:foo
git push origin foo:main
```

### 2.6 Fetch arguments 
![image](https://github.com/user-attachments/assets/e3127649-6639-41fd-aae6-647744b79249)

```sh
git fetch origin main~1:foo
git fetch origin foo:main
git checkout foo
git merge c6
```

### 2.7 Source of nothing  
![image](https://github.com/user-attachments/assets/1801ba39-6963-4f18-860a-3aa0ededdd37)

```sh
git push origin :foo
git fetch origin :bar
```

### 2.8 Pull arguments 
![image](https://github.com/user-attachments/assets/2017017e-7c86-4021-91f8-22659b5fbc0f)
 
```sh
git pull origin bar:foo
git pull origin main:side
```
