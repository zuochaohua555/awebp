# AWebp

animated webp 小工具(笨方法)

```shell
> npm i -g awebp
> awebp -h

  -h --help                                      显示帮助
  -d --dispose [method] [file] [outFile]         dispose-method: 0 for NONE or 1 for BACKGROUND
  -q --quality [quality] [file] [outFile]        Specify the compression between 0 and 100
  -e --extract-frame [file] [outDir]             提取帧出来

Examples:
  awebp -d 0 ./test/test.webp            // 设置webp每帧的dispose method为0
  awebp -q 75 ./test/test.webp           // 设置动图webp压缩率, 提取帧->转png->重新拼接webp
  awebp -e ./test/test.webp frames       // 提取所有帧出来到frames文件夹
```

# 使用场景

1. ffmpeg 转换出来的 webp 重叠问题, 需要设置 dispose-method 为 BACKGROUND
2. animated webp 压缩

# TODO

1. 兼容其他操作系统
