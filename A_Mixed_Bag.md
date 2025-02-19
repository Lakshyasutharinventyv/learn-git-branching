# 1 Introduction Sequence
### 1.1 Introduction to Git Commits

![image](https://github.com/user-attachments/assets/45bc85c4-3e4f-4246-a31e-ba4102da42fc)


```
git commit
git commit
```

### 1.2 Branching in Git

![image](https://github.com/user-attachments/assets/8d441a5e-2e38-4a20-bfa6-f4c6fff82640)

```
git branch bugFix
git checkout bugFix
```

### 1.3 Merging in Git

![image](https://github.com/user-attachments/assets/062130df-99d1-4026-806b-b866bae507fe)

```
git checkout -b bugFix    
git commit  
git checkout main
git commit
git merge bugFix
```

### 1.4 Rebase Introduction

![image](https://github.com/user-attachments/assets/306e42aa-a3cf-4bb3-baea-55ba0089faba)

```
git checkout -b bugFix    
git commit    
git checkout main    
git commit    
git checkout bugFix    
git rebase main
```
