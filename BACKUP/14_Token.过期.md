# [Token 过期](https://github.com/gnimg/gitblog/issues/14)

当你的`personal access token`过期的时候，当然，你的`Action`就没办法成功完成啦。

`Generate README` action会遇到如下的错误：
```
github.GithubException.BadCredentialsException: 401 {"message": "Bad credentials", "documentation_url": "https://docs.github.com/rest"}
Error: Process completed with exit code 1.
```

### 解决办法

1. 首先，当然你需要更新Token。根据自己的需要，选择一个有效期。
2. **敲桌板** - regenerate token以后，务必要更新 `repo` 里面的 `secrets`。
3. Re-run action即可。

