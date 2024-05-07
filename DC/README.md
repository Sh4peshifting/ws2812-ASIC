# DC综合

## 使用方法
1. 确保 `synopsys_fm.setup` 中的变量指向正确的文件或目录
2. 确保 `scripts` 目录中的脚本中 `TOP_MODULE` `search_path`变量指向正确
3. 根据需要修改 `scripts/constraints_compile.tcl` 脚本中的约束
4. 先运行 `run_dc_read_rtl.sh` 读取设计，然后运行 `run_dc_constraint_compile.sh` 

## 备注
- `clean.sh` 用于清理生成的文件
- `reports` 目录中存放了综合报告，包括面积、时序、功耗估值等