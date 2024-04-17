# LBLTNewCore
A fork of [LinearPurpur](https://github.com/StupidCraft/LinearPurpur) that adds support for the [Linear region file format](https://github.com/xymb-endcrystalme/LinearRegionFileFormatTools).

> ⚠️ **99% of plugins should be functional, except plugins that need to directly access the `.mca` files.**

# Configuration
All configuration regarding LBLTNewCore is stored in Purpur's `purpur.yml` file, you may need to manually add in these configuration options
if you are replacing Purpur with LBLTNewCore or delete the `purpur.yml` file to allow it to re-generate.

### Global Configuration
```yml
region-format:
  linear:
    flush-frequency: 10
    flush-max-threads: 1
```

### Per-world Configuration
```yml
region-format:
  format: ANVIL # Change this to "LINEAR" to use Linear region file format.
  linear:
    compression-level: 1
    crash-on-broken-symlink: true
```

# Compiling
1. #### Clone LinearPurpur
```sh
git clone https://github.com/StupidCraft/LinearPurpur.git
```
2. #### Apply Patches
```sh
./gradlew applyPatches
```
3. #### Create Paperclip Jar
```sh
./gradlew createReobfPaperclipJar
```

You will find a compiled Paperclip Jar file in `build/libs/`.

# Credits
- [**Leleawa**](https://github.com/Leleawa) - skid LinearPurpur.

  # 中文翻译：
  # LBLTNewCore
- 一个叉子来自[LinearPurpur](https://github.com/StupidCraft/LinearPurpur) 然后增加支持对[Linear region file format](https://github.com/xymb-endcrystalme/LinearRegionFileFormatTools).

> ⚠️ **99%的插件都应该能正常运作，除非有神秘插件直接访问`.mca`文件.**
>
## 配置

关于LBLTNewCore的所有配置都存储在Purpur的 `Purpur.yml` 文件中，您可能需要手动添加这些配置选项，如果您要用LBLTNewCore替换Purpur，或者删除 `Purpur.yml` 文件以允许其重新生成。

### 全局配置

```yml
region-format:
  linear:
    flush-frequency: 10
    flush-max-threads: 1
```

### 世界配置
```yml
region-format:
  format: ANVIL # 修改这个为"LINEAR"来使用线性区域文件格式。
  linear:
    compression-level: 1
    crash-on-broken-symlink: true
```

# 编译
1. #### 克隆 LBLTNewCore
```sh
git clone https://github.com/StupidCraft/LinearPurpur.git
```
2. #### 应用补丁
```sh
./gradlew applyPatches
```
3. #### 创建 Paperclip Jar
```sh
./gradlew createReobfPaperclipJar
```


你将在`build/libs`找到一个编译后的Paperclip Jar文件

# Some patches from | 一些补丁来自
Polpot (https://github.com/HaHaWTH/Polpot)

PandaSpigot (https://github.com/hpfxd/PandaSpigot)

Tuinity (https://github.com/Tuinity/Tuinity)

Mirai (https://github.com/etil2jz/Mirai)

Gale (https://github.com/GaleMC/Gale)
