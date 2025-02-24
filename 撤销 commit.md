### 还未推送到远端

```bash
# 保留修改，但撤销 commit
git reset --soft HEAD^

# 或者指定具体要回退到的 commit
git reset --soft commit_hash
```

### 已推送到远端

```bash
# 查看 log
git log --oneline

# 撤销最后一次 commit
git revert HEAD
输入 :wq 保存并退出

# 撤销指定的 commit
git revert commit_hash
```



### 提交类型
* feat: 新功能
* fix: 修复 bug
* docs: 文档更新
* style: 代码格式修改，不影响代码逻辑
* refactor: 代码重构
* test: 测试用例相关
* chore: 构建过程或辅助工具的变动
* perf: 性能优化