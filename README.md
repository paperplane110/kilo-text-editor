# Text editor `Kilo` by C

Build your own text editor for learning C: [tutorial](https://viewsourcecode.org/snaptoken/kilo/index.html)

## Build

```bash
# go to the project file
cd kilo

# compile kilo.c
make
```

Then you will find `./kilo` inside the current dir.

## Usage

```
# Open an empty editor
./kilo

# Open a file
./kilo <filename>

# Quit
Ctrl + q

# Save
Ctrl + s

# Quit without saving
Ctrl + q + q + q
```

## Note

### 1. `sprintf` and `snprintf`

两者都是将数据写入缓冲区，并且返回缓冲区的长度（不包含结束符`\0`）。
两者的区别在于 `snprintf` 要求提前声明要写入的数组长度，更加安全。

```c
int num = 3;
char buf[5];
int len1;
int len2;

len1 = snprintf(buf, sizeof(buf), "1+2=%d", num);
len2 = sprintf(buf, "1+2=%d", num);
```

## Other links:

- C operators: [link](https://www.runoob.com/cprogramming/c-operators.html)
- C array of pointers: [link](https://www.runoob.com/cprogramming/c-array-of-pointers.html)
- `<termios.h>`: [link](https://blog.csdn.net/qq_53144843/article/details/126611199?spm=1001.2101.3001.6650.6&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ERate-6-126611199-blog-4105607.pc_relevant_aa2&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ERate-6-126611199-blog-4105607.pc_relevant_aa2&utm_relevant_index=7)
- `<unistd.h>`: [link](https://blog.csdn.net/reasonyuanrobot/article/details/103172210)
- Console colors: [link](https://gist.github.com/abritinthebay/d80eb99b2726c83feb0d97eab95206c4)
- Console codes: `man console_codes` or [link](https://blog.51cto.com/u_1923895/5939748)
- Static variables: [link](https://www.geeksforgeeks.org/static-variables-in-c/)
