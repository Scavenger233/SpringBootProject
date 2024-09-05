## How to push codes to github
要将 IntelliJ IDEA Ultimate 上的代码同步到 GitHub 上，可以按照以下详细步骤操作，适用于 Mac 电脑。

### 前提条件：
1. 你需要一个 **GitHub 账号**。
2. 在 GitHub 上已经创建了一个仓库，或者准备将代码推送到新仓库。
3. 安装了 **Git**，一般 IntelliJ 已经集成了 Git。

### 详细步骤：

#### 1. 设置 IntelliJ 与 GitHub 关联
- 打开 IntelliJ IDEA。
- 点击左上角的 `IntelliJ IDEA` 菜单 -> `Preferences`（或者按 `⌘ + ,`）。
- 选择 `Version Control` -> `GitHub`。
- 在 `GitHub` 界面中，点击 `+` 号，输入你的 GitHub 账户并授权 IntelliJ 访问 GitHub。

#### 2. 初始化 Git 仓库
- 如果你的项目还没有 Git 仓库，点击顶部菜单中的 `VCS` -> `Enable Version Control Integration...`。
- 选择 `Git`，这将初始化一个 Git 仓库。
- 项目中会出现 `.git` 文件夹，这表示项目已经被 Git 管理。

#### 3. 将项目提交到本地仓库
- IntelliJ 会自动检测代码的修改。如果有未跟踪的文件，在 `Project` 面板中，它们会以蓝色高亮显示。
- 提交代码：右键点击 `Project` 窗口中未提交的文件，选择 `Git` -> `Add`，将文件添加到 Git 的暂存区。
- 接下来，点击右上角的 `Commit` 按钮，输入提交信息，确认后点击 `Commit` 按钮。
  - 如果希望在提交时运行代码检查，也可以选择 `Commit and Push`，直接提交并推送到远程仓库。

#### 4. 将本地仓库推送到 GitHub
- 在 IntelliJ 中创建远程仓库链接：
  - 点击顶部菜单中的 `VCS` -> `Git` -> `Remotes`。
  - 点击 `+`，然后将你 GitHub 仓库的 URL 填入。GitHub 仓库 URL 可以在 GitHub 网站的仓库页面中找到，点击 `Code` 按钮，选择 `HTTPS`，然后复制地址。

- 推送代码到 GitHub：
  - 点击顶部菜单中的 `VCS` -> `Git` -> `Push`，或者按快捷键 `⌘ + Shift + K`。
  - 在弹出的窗口中，选择要推送的分支和远程仓库（默认是 `origin`）。
  - 点击 `Push` 按钮，IntelliJ 会将你的代码推送到 GitHub。

#### 5. 验证推送是否成功
- 打开你的 GitHub 账户，进入相应的仓库页面。
- 你应该可以看到刚刚从 IntelliJ 推送的代码。

### 如果没有远程仓库，创建一个新的仓库
1. 登录 GitHub。
2. 点击右上角的 `+` 按钮 -> `New repository`。
3. 填写仓库名称和描述，然后点击 `Create repository`。
4. 使用仓库的 URL 进行远程设置，然后按照上面推送代码的步骤将本地项目推送到新的仓库。

### 通过 GitHub Desktop 操作（可选）
1. 打开 GitHub Desktop，点击 `File -> Add Local Repository`。
2. 选择 IntelliJ 项目的文件夹，点击 `Add`.
3. GitHub Desktop 会显示所有更改，点击 `Commit` 按钮进行提交。
4. 然后点击 `Push origin` 将代码推送到 GitHub。

这样，你的代码就会成功同步到 GitHub 上了。

有其他问题可以继续问我！
