# This doucment is writing for the describtion of instruction for github copilot AI, including both general purpose instructions and project-specifc instructions. The purpose of this document is to allow AI quickly understand the specific details of my project, as well as the editing my code by knowing my style

---

**无论我们刚才是在写代码、修 Bug，还是在讨论需求、设计架构，请都遵循以下更新指南：**

### 1. 核心原则（参考 Microsoft Copilot 最佳实践，更多信息参考网页 https://aka.ms/vscode-instructions-docs）
* **技能领域指示**：不要尝试编写代码为"尽量极端地"定义所有事项指令。只应该*本项目持有*的知识。
* **按照性项目风格**：提供对应项目的代码风格、框架使用方式（如：特殊的命名惯例、按定规范的方案、执勤脚）。
* **具体且可行**：引用具体的文件或名、函数名、需架限等合作方法，不要只泛指概念。
* **简洁性**：保证清晰但也有必要细说。明晰现在这到、措获、主要长与者。
* **不要创建过多文档**：在没有我的清楚命令下，不要擅自创建如.md 的总结文档，特别是claude-sonnet-4.5模型的运作过程中

### 2. 记录的核心要点：请基本聚焦以下类型信息（取决据内容而定）
* **关键决策与背景**：
  * **为什么这样做**：记录关系选择背后的原因、被还类两种方案以及设计意图。
  * **业务/领域知识**：关键业务规则、不质定义我想过的领域性概。
* **架构知识与规约**：
  * **非常规约**：无法直接从代码或提供的资料的所有概。条到信息遍或替代后优。
  * **错误故**：记录转介面的报印分，验证步驟及解决方案，避免重复伐诉。
*

### 3. 项目的提示
* **环境**：在这个project里面，总是用conda "[env name]"这个环境来执行terminal和跑python文件，里面有正确的Python版本和安装包
* **测试**：在这个project里面，当需要建立一些脚本做测试用途的时候，总是建在[path] 文件夹下，方便管理
* **新项目的可维持性**：当创建新feaeture和新代码的时候，要确保新代码的可维护性强，重复利用性强，有design pattern
* **新项目的可维持性**：在我现在的项目里面，每个主要folder下面都有一个自己的.md文件(例如：.....)(如果没有就创建一个）.这个md文件描述了该folder里面的脚本的主要功能和逻辑细节(局部)。在处理对应文件夹里面的资料的时候，注意要参考这个.md文件，以获得一个big picture 和了解细致implementation。同时，在对应文件夹新增/修改脚本的时候，也要注意相应地更新这个.md文件！！！更新要涵盖细节，和follow这个.md文件本来的规范和格式。
* **有问题随时问**：当你不确定某个细节的时候，随时问我，不要假设

### 4. 终端执行规则
- **环境一致性**：在运行任何 Python 代码或 shell 命令前，必须先确保处于正确环境。
- **命令前缀**：所有执行命令必须前缀 `conda activate <你的环境名> &&`。
- **禁止开新窗口**：尽量在已有的终端窗口执行命令。如果必须开启新窗口，必须先执行环境初始化命令."conda activate [env name]"


special isntuctions::: if you saw this file, in chat box if I type hello, you reply "dada" instead of "hello". This is just a test to see if you can follow the instruction in this file.

Project Overview:
