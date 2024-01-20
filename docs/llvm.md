# LLVM

## CMD
### Setup
```bash
cmake -S llvm -B build -G Ninja -DCMAKE_BUILD_TYPE=Release
ninja -C build [build project]
```

### Other
```bash
# LLVM IR .bc
clang <source-file or assembly-file> -emit-llvm -c -o <output-file>
# LLVM IR .ll
clang <source-file or bitcode-file> -emit-llvm -S -c -o <output-file>
# Disable O0 optnone
clang -S -emit-llvm ../inputs/input_for_hello.c -Xclang -disable-O0-optnone  -o input_for_hello.ll
# opt
opt -time-passes -O<level> <bitcode-file or assembly-file> -o <bitcode-file>
opt -O<level> <bitcode-file or assembly-file> -S -o <assembly-file>
```

