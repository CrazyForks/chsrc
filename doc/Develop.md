<!-- -----------------------------------------------------------
 ! SPDX-License-Identifier: GFDL-1.3-or-later
 ! -------------------------------------------------------------
 ! Doc Type      : Markdown
 ! Doc Name      : 01-Develop.md
 ! Doc Authors   : Aoran Zeng <ccmywish@qq.com>
 ! Contributors  :  Nul None  <nul@none.org>
 !               |
 ! Created On    : <2024-12-27>
 ! Last Modified : <2024-12-27>
 ! ---------------------------------------------------------- -->

# 开发

## 环境

请安装好 `GCC` 或 `Clang` 和 `make` 以及 `curl`

```bash
# 请务必使用 dev 分支开发
$ git clone https://gitee.com/RubyMetric/chsrc.git -b dev
```

<br>

## 编译运行

```bash
$ make          # 默认使用 cc 编译
$ make CC=clang # 使用 clang 编译
$ make CC=gcc   # 使用 gcc   编译
```

```bash
# 编译并直接启动 GDB
$ make debug

# 如果需要单独生成含有编译信息的二进制文件（这个不会自己启动GDB）
$ make DEBUG=1
```

<br>

## 测试

```bash
$ make test-xy  # 测试 xy.h
$ make test-fw  # 测试 framework
$ make test     # 测试上述两个
$ make test-cli # 测试命令
$ make clean
```

<br>

## 提交 PR

关于分支的说明以及如何提交代码，请参考 [./CONTRIBUTING.md](./CONTRIBUTING.md)

<br>