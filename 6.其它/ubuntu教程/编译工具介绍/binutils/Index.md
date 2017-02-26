# binutils

GNU binutils是一组二进制工具集。包括：addr2line ar gprof nm objcopy objdump ranlib size strings strip. 本文归纳他们的常用法。ar用于建立、修改、提取档案文件(archive)。archive是一个包含多个被包含文件的单一文件（也称之为库文件），其结构保证了可以从中检索并得到原始的被包含文件（称之为archive中的member）。member的原始文件内容、模式（权限）、时间戳、所有者和组等属性都被保存在 archive中。member被提取后，他们的属性被恢复到初始状态。