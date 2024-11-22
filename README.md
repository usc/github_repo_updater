# github仓库更新检查

## 使用
```
python main.py --file repo.txt --days 7 --cache cache.json
```
参数说明：
```
token：GitHub 的个人访问令牌，从 .env 文件获取 GitHub token。
--file：仓库列表文件路径，默认为 repo.txt。
--days：检查的时间范围，默认为过去 7 天。
--cache：缓存文件，默认缓存文件为 cache.json。
```

## 优势
- 支持自定义的仓库：仓库列表文件自维护
- 避免重复提醒：缓存记录所有提示过的版本，确保同一版本不会重复输出。
- 支持多版本发布：可以在同一时间窗口内识别并提示多个新版本。
- 持久化记录：缓存存储在本地文件中，即使程序重启也能维持状态。