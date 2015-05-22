##自动化测试

如果你想构建可靠的高质量的软件，自动化测试将是你工具箱里面非常关键的一个部分，它帮助你减少手工测试的代价，提高你的开发小组重构已有代码的能力。

###自动化测试的类型

　并非所有的自动化测试都是相似的，他们通常在作用域、实现方式和执行时间上有所差异，我把他们分成三种类型的测试：单元测试、集成测试和功能测试。

* 单元测试用于测试你代码的最小单元，在基于java的项目中这个单元就是一个方法(method)，在单元测试中你会避免与其他类或者外部的系统打交道。单元测试很容易编写，执行起来非常快速，能够在开发阶段给你代码的正确性提供反馈。
* 集成测试用于测试某一个组件或者子系统。你想确保不同类之间的交互能够按照预期一样，一个典型的情况就是逻辑层需要和数据库打交道。因此相关的子系统、资源文件和服务层必须在测试执行阶段是可访问的。集成测试通常比单元测试运行更慢，更难维护，出现错误时也比较难诊断。
* 功能测试用于测试一个应用的功能，包括和外部系统的交互。功能测试是最难实现也是运行最慢的，因为他们需要模仿用户交互的过程，在web开发的情况，功能测试应该包括用户点击链接、输入数据或者在浏览窗口提交表单这些情形，因为用户接口可能随着时间改变，功能测试的维护将会很困难。

###自动化测试金字塔

你可能想知道到底哪一种测试最适合你的项目，在现实环境中你可能会混合使用这几种测试方法来确保你的代码在不同架构层面都是正确的。你需要写多少测试取决于编写和维护测试的时间消耗。测试越简单就越容易执行，一般来讲你的项目应该包含很多单元测试，少量的集成测试以及更少的功能测试。




