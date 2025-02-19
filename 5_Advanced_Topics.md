# 5. Advance Topics

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
