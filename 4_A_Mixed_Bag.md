# 4. A Mixed Bag

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
