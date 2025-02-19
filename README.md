
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

## 2. Navigating Git History

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

## 3. Advanced Git Operations

### 3.1 Cherry-pick Intro

![image](https://github.com/user-attachments/assets/e734ebf0-1a12-4e5d-85ef-0d5bd121d87d)

```
git cherry-pick C3 C4 C7
```

### 3.2 Interactive Rebase Intro

![image](https://github.com/user-attachments/assets/d28de05b-5e91-4dd7-aa26-798ff0d7c785)

```
git rebase -i main~4 --aboveAll
// Remove C2, move C5 up
```

## 4. Handling Individual Commits

### 4.1 Grabbing Just One Commit

![image](https://github.com/user-attachments/assets/dec383e5-6652-4044-9ae4-faab2b694119)

```
git checkout main
git cherry-pick C4
```

### 4.2 Juggling Commits

![image](https://github.com/user-attachments/assets/e289fd0b-5aef-4fe1-aaa3-cb951178416d)

```
git rebase -i HEAD~2
git rebase -i HEAD~1
git rebase -i HEAD~2
git branch -f main caption
```

### 4.3 Juggling Commits #2

![image](https://github.com/user-attachments/assets/708d1a66-e5eb-46d5-be8e-19a414dfa940)

```
git checkout main
git cherry-pick C2
git commit --amend
git cherry-pick C3
```

### 4.4 Git Tags

![image](https://github.com/user-attachments/assets/5da02858-e6cb-4fe7-a1e7-e2532a75d9a5)

```
git tag v0 C1
git tag v1 C2
git checkout C2
```

### 4.5 Git Describe

![image](https://github.com/user-attachments/assets/7d6fb196-df04-4222-9f97-359580150a90)

```
git commit
```

## 5. Complex Git Scenarios

### 5.1 Rebasing Multiple Times

![image](https://github.com/user-attachments/assets/debdf61f-fc8d-4fb7-b7c6-ad746ffcf282)

```
git rebase main bugFix
git rebase bugFix side
git rebase side another
git rebase another main
```

### 5.2 Multiple Parents

![image](https://github.com/user-attachments/assets/c5f93ff4-542c-4053-ba22-8a604899e763)

```
git branch bugWork main~^2~
```

### 5.3 Branch Spaghetti

![image](https\://github.com/user-attachments/assets/adac4496-86e7-4749-b4fd-fedc7da3b238)

```
git checkout one
git cherry-pick C4 C3 C2
git checkout two
git cherry-pick C5 C4 C3 C2
git branch -f three C2
```
