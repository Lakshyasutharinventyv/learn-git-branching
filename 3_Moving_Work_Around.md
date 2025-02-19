# 3. Moving Work Around
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

