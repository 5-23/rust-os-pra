# rust-os-pra
[강의영상](https://www.youtube.com/watch?v=rH5jnbJ3tL4&list=PLib6-zlkjfXkdCjQgrZhmfJOWBk_C2FTY)을 보면서 러스트로 os를 만드는방법을 연습할 예정입니다.

## build

```fish
# Linux
cargo rustc -- -C link-arg=-nostartfles

# Windows
cargo rustc -- -C link-args="/ENTRY:_start /SUBSYSTEM:console"

# macOS
cargo rustc -- -C link-args="-e __start -static -nostartfiles"f
```