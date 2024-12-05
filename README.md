# cpp-git-hooks
My git hooks for cpp.

## Usage

You can add this as a submodule for your project. Execuate the command on your root directory of your project

```bash
git submodule add https://github.com/yibotongxue/cpp-git-hooks.git hooks
```

Initialize and update it

```bash
git submodule update --init --recursive
```

Then set the `core.hooksPath`

```bash
git config core.hooksPath ./hooks/hooks
```
