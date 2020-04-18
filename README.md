# LinkGame
## Android:连连看

#### 第一次commit-2020-04-15:
- 项目基础操作。
- 自定义XLTextView和XLButton类，方便设置其字体样式为指定的字体样式。
- 成功，失败界面搭建。
- 文件结构调整。
- 数据库创建（第三方库：[Litepal](https://github.com/LitePalFramework/LitePal)）。

#### 第二次commit-2020-04-15：
- 数据库更新操作，使用可视化工具Navicate for Sqlite问题重重。
- 工具类，dp与px之间的转换。

#### 第三次commit-2020-04-16-00:06：
- 首页布局。
- 状态栏的沉浸模式（第三方库：[ImmersionBar](https://github.com/gyf-dev/ImmersionBar)）。
- 常量文件以及一些枚举的定义，设置枚举值以及测试。
- 数据库可视化依赖（第三方库：[Android-Debug-Database](https://github.com/amitshekhariitbhu/Android-Debug-Database)）。
- 数据库查询操作（注意DataSupport已经废弃，模型类需要继承于LitePalSupport）。
- 数据库查询测试。

#### 第四次commit-2020-04-17-19:10：
- 枚举的完善。
- Activity跳转，携带自定义类的数据。针对数据模型类，实现Serializable接口或Parcelable接口接口。
- 关卡页面布局。
- 自定义XLImageView，显示不同关卡状态的图片。
- 完善工具类：获取屏幕宽度，高度。

#### 第五次commit-2020-04-18-09:43：
- 关卡页面bug解决。不是Horizontal无法嵌套RelativeLayout而是计算页面的时候理论上应该这样计算`int pager = i / Constant.level_pager_count;`，但是最终写成了对`level_width`取整。
- 创建了游戏界面，关卡界面到游戏界面的数据传递已经完成。
- 注意：游戏界面到数据界面的回调数据还没有完成。
