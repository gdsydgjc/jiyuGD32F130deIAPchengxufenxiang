# 基于GD32F130的IAP程序

## 简介

本资源提供了一套完整的基于GD32F130微控制器的在应用编程（In-Application Programming，简称IAP）解决方案。GD32F130系列是瑞萨电子GD32系列中的高性能成员，广泛应用于嵌入式系统开发。此程序包精心设计，旨在帮助开发者实现固件的在线升级功能，无需外部编程器，大大简化了产品维护和功能扩展的过程。

## 包含内容

- **Bootloader程序**：启动加载器，负责接收并处理升级请求，通过串口利用YMODEM协议从宿主机接收新的应用程序固件。

  - **App示例程序**：演示如何编写可被更新的应用程序部分，包含基本的入口点和必要的初始化代码，供开发者理解如何构建应用程序以兼容IAP机制。

  - **文档说明**：简要指导用户如何烧录bootloader、配置以及使用IAP功能的说明文档。

  ## 特性

  - **兼容性强**：不仅适用于GD32F130，其设计思路和大部分代码亦可供其他GD32系列芯片的IAP项目作为参考。

    - **YMODEM协议**：选择了经典的YMODEM协议进行固件传输，稳定可靠，适用于资源有限的嵌入式环境。

    - **易于集成**：清晰的模块化结构使得该IAP方案能够轻松集成到现有的GD32项目中，提升固件升级体验。

    ## 使用指南

    1. **准备工作**：确保开发环境已搭建完成，推荐使用RISC-V或ARM编译工具链。

       2. **编译与烧录**：首先编译并烧录bootloader至MCU的特定区域，随后根据文档指示操作，将app示例或者您的应用程序烧录至预留区域。

       3. **测试验证**：通过串口发送固件更新指令，验证IAP流程是否正常工作，即旧固件能否成功被新固件替换。

       ## 注意事项

       - 请严格按照提供的文档步骤操作，避免固件损坏。
       - 考虑到不同版本的IDE和编译器可能存在的差异，请适当调整编译设置。
       - 本资源仅供学习交流使用，商业用途请咨询相关版权和许可问题。

       加入GD32的探索之旅，利用这套IAP程序包，您的设备将获得更加灵活的固件管理能力，提高产品的市场适应性和竞争力。祝您开发顺利！

       ## 下载链接
       [基于GD32F130的IAP程序分享](https://pan.quark.cn/s/c693202d012d) 

       (备用: [备用下载](https://pan.baidu.com/s/18sznTenbz02p60K7HSwEfA?pwd=1234))

       ## 说明

       该仓库仅用于学习交流，请勿用于商业用途。
