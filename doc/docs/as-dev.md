## 辅助开发

FIS3 提供**文件监听**和**livereload**两种辅助开发工具。

### 文件监听

文件监听有效的提升开发效率，你不需要每次修改资源就执行 `fis3 release` 来编译发布，而其自动监听文件变化，每次文件变化都会重新编译此文件以及**依赖**它的文件。除了方便开发以外，还有效的提升了编译效率。

通过给 [command#release][] 命令添加 `--watch`（或简写`-w`） 参数来启用此功能。

```bash
fis3 release --watch
```

### livereload

livereload 一般和文件监听功能一起使用，当文件发生变化时，自动刷新页面。这个功能也很有效，特别是在做页面微调的时候。

通过给 [command#release][] 命令添加 `--live`（或简写`-L`） 参数来启动此功能。

[command#release]: ./command.md#release