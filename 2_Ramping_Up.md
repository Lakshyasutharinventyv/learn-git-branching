# 2. Ramping Up

### 2.1 Detach HEAD

![image](https://github.com/user-attachments/assets/51298e3b-4f4b-4d78-9528-069c9f3dffee)

```
git checkout C4
```

### 2.2 Relative Refs (^)

![image](https://github.com/user-attachments/assets/bfa46a0c-b4c1-4339-a84f-06bd6d4dbe34)

```
git checkout C4^
```

### 2.3 Relative Refs (\~)

![image](https://github.com/user-attachments/assets/4ca667e1-c1a3-455b-8866-0b3ffd30129e)

```
git branch -f main C6
git branch -f bugFix C0
git checkout C1
```

### 2.4 Reversing Changes in Git

![image](https://github.com/user-attachments/assets/960aaf0b-ed15-4118-96e3-028535ca5e8c)

```
git reset local~1
git checkout pushed
git revert pushed
```

