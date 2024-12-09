# My Git Hooks

这是我的 `git` 钩子的托管仓库，包含一些常用的项目类型的 `git` 钩子，当前支持用 `CMake` 或 `XMake` 管理的 `C++` 项目；`Cuda`项目。

## `CMake` 或 `XMake` 管理的 `C++` 项目

相关的脚本在 `cpp-hooks` 下，使用方法可以是将其中的脚本拷贝到 `.git/hooks/` 下使用，或者将其中的脚本下载到你喜欢的文件夹，比如项目根目录下的 `hooks` 文件夹，然后执行下面的命令

```bash
git config core.hooksPath ./hooks
```

> [!TIP]
> 对于 `CMake` 和 `XMake` 的要求仅仅是在 `pre-push` 钩子中，如果不是使用这两个构建系统，可以选择删除 `pre-push` 钩子。

## `Cuda` 项目

相关的脚本在 `cuda-hooks` 下，与 `C++` 项目的相比没有使用 `pre-push` 钩子，因而对构建系统没有要求，具体使用方法参考 `C++` 项目，也就是将其中的脚本拷贝到 `.git/hooks/` 下使用，或者将其中的脚本下载到你喜欢的文件夹，比如项目根目录下的 `hooks` 文件夹，然后执行下面的命令

```bash
git config core.hooksPath ./hooks
```

## `Python` 项目

相关的脚本在 `python` 下，使用方法可以是将其中的脚本拷贝到 `.git/hooks/` 下使用，或者将其中的脚本下载到你喜欢的文件夹，比如项目根目录下的 `hooks` 文件夹，然后执行下面的命令

```bash
git config core.hooksPath ./hooks
```

## TODO

- [x] `XMake` 管理的 `C++` 项目
- [x] `Cuda` 项目
- [x] `Python` 项目
- [ ] 修正 `pre-merge-commit` 钩子
- [ ] 增加文档说明和配置文件
