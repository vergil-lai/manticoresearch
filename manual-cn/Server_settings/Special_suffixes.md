# 特殊后缀

Manticore Search 支持使用特殊后缀，以简化具有特定含义的数值。这些后缀分为大小后缀和时间后缀。后缀的常见格式为 `整数` 后跟 `字面量`，例如 `10k` 或 `100d`。字面量不区分大小写，因此 `10W` 和 `10w` 被视为相同。

- 大小后缀：这些后缀可用于定义某物大小的设置，如内存缓冲区、磁盘文件大小或 RAM 限制。如果未指定后缀，默认情况下值将视为字节。可用的大小后缀包括：
  - `k` 表示千字节（1k = 1024 字节）
  - `m` 表示兆字节（1m = 1024k）
  - `g` 表示千兆字节（1g = 1024m）
  - `t` 表示太字节（1t = 1024g）
- 时间后缀：这些后缀可用于定义时间间隔值的设置，如延迟或超时。未加修饰的值通常有文档记录的刻度，但您可以使用明确的后缀来避免猜测。可用的时间后缀包括：
  - `us` 表示微秒
  - `ms` 表示毫秒
  - `s` 表示秒
  - `m` 表示分钟
  - `h` 表示小时
  - `d` 表示天
  - `w` 表示周

<!-- proofread -->