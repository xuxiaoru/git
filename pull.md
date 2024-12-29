在 Linux 上首次克隆远程仓库指定分支，并在后续拉取更新，你可以按照以下步骤操作：

### 1. **首次克隆远程仓库并指定分支**

假设你要克隆的远程仓库 URL 是 `https://github.com/username/repository.git`，并且你希望克隆指定的分支（例如 `feature-branch`）。你可以使用以下命令：

```bash
git clone -b feature-branch https://github.com/username/repository.git
```

其中：
- `-b feature-branch`：指定克隆的分支为 `feature-branch`。
- `https://github.com/username/repository.git`：是你要克隆的远程仓库的 URL。

这个命令将会克隆指定分支的代码到本地。

### 2. **进入本地仓库目录**

克隆完成后，进入仓库目录：

```bash
cd repository
```

### 3. **后续拉取更新**

在首次克隆并进入本地仓库目录后，你可以使用 `git pull` 拉取更新。假设你仍然希望拉取 `feature-branch` 分支的更新，可以使用以下命令：

```bash
git pull origin feature-branch
```

这将会拉取远程 `origin` 仓库中的 `feature-branch` 分支的最新更新到本地。

### 4. **切换到其他分支并拉取更新（可选）**

如果你需要切换到仓库中的其他分支并拉取更新，可以先使用 `git checkout` 切换分支，然后使用 `git pull` 拉取该分支的更新。例如：

```bash
git checkout other-branch  # 切换到其他分支
git pull origin other-branch  # 拉取其他分支的更新
```

### 总结：
1. **首次克隆指定分支**：`git clone -b <branch_name> <repository_url>`
2. **拉取指定分支的更新**：`git pull origin <branch_name>`
3. **切换分支并拉取更新**：`git checkout <branch_name>`，然后 `git pull origin <branch_name>`

这样，你就可以在 Linux 上克隆指定分支并保持后续更新。如果有其他问题，请随时告诉我！
