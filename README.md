# Dev-Utils
Common development utils such as format styles, coding guidelines etc.

## Setup
Simply clone this repository and execute the `init_dotfiles.sh` script like so:

```
$ git clone https://github.com/NewProggie/Dev-Utils.git
$ cd Dev-Utils && bash init_dotfiles.sh
```

## Customizations
One may has some settings to make which are exclusively bound the current used
setup such as workplace or home. For those kind of settings there are two extra
files which get sourced but do not belong to version control: `.extra` `.path`.

For `.path` some typical settings might be:

```
# Add LLVM tools to PATH variable
export PATH="$HOME/Projekte/llvm/build/bin:$PATH"
export DYLD_LIBRARY_PATH="$HOME/Projekte/llvm/build/lib:$DYLD_LIBRARY_PATH"

export CLANG_FORMAT_PATH="${LLVM_REPO}/tools/clang/tools/clang-format"
export CLANG_INCLUDE_FIXER_PATH="${LLVM_REPO}/tools/clang/tools/extra/include-fixer/tool"
export CLANG_RENAME_PATH="${LLVM_REPO}/tools/clang/tools/extra/clang-rename/tool"
```

Other stuff such as gnupg settings, environment variables etc. belong to
`.extra`.
