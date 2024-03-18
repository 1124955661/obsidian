---
title: 未命名
date created: 2024-03-18T10:25:40
date modified: 2024-03-18T10:27:43
---

```dataview
list
from ""
where contains(file.tags,"python")
```

| item             | type         | description                                                                                                       |
| ---------------- | ------------ | ----------------------------------------------------------------------------------------------------------------- |
| file.path        | string 字符串   | 文件的路径（相对于整个 Vault）                                                                                                |
| file.folder      | string 字符串   | 文件所属的文件夹的路径（相对于整个 Vault）                                                                                          |
| file.name		<br>  | string 字符串   | 文件名                                                                                                               |
| file.link        | link         | 引用这篇文件时的链接                                                                                                        |
| file.outlinks    | link         | 该文件外链                                                                                                             |
| file.inlinks     | link         | 指向本文的文件的链接                                                                                                        |
| file.etags       | string 字符串   | 该文件的所有标签 <br>例如文件中有标签 #A/B ，只会有 #A/B；<br>file.tags	string 字符串	该文件的所有标签，以及他们的各级标签<br>例如文件中有标签 #A/B ，就会有 #A/B 和 #A； |
| file.aliases     | string       | 别名，添加元数据直接覆盖即可，可以取多个；<br>例如在 frontmatter 中写 aliases: [别名1, 别名2]                                                   |
| file.lists       | object 对象    | 文件中出现的所有列表的信息（任务是特殊的列表）                                                                                           |
| file.tasks       | object       | 文件中出现的所有任务的信息                                                                                                     |
| file.ext         | string 字符串   | 文件的拓展名（ext 是 extension 的缩写）                                                                                       |
| file.frontmatter | object 对象    | 前言中的元数据                                                                                                           |
| file.ctime	date  | 时间类型         | 文件的创建时间（c 代表 create 创建）                                                                                           |
| file.mtime       | date 时间类型    | 文件最后修改时间（m 代表 modify 修改）                                                                                          |
| file.size        | number 数字    | 文件的大小（单位为 byte）                                                                                                   |
| file.starred     | boolean 布尔类型 | 文件是否被星标（核心插件星标已经被书签替代）<br>该属性无法被覆盖，书签标记也无法令其为 true                                                                |
|                  |              |                                                                                                                   |












