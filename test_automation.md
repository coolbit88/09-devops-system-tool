## 自动化测试

### 1. 代码质量管理

代码质量管理xxxx。

##### 应包含以下基本功能：

——xxxx

——xxxx

##### 可以包含以下高级功能：

——xxxx

——xxxx
### 1. 静态代码检查
静态代码检查是持续交付流水线中的一个重要环节，利用商用/开源/自研的代码检查工具在开发阶段发现缺陷，让缺陷在最短路径闭环。

##### 应包含以下基本功能：

——对代码进行静态扫描，发现代码缺陷、安全漏洞及编程规范、重复代码、复杂度高等代码坏味道问题

——能够自动触发/立即分析/定时开展，实时展示扫描进展状态，及时反馈代码检查结果

——方便查看告警及错误代码片段，提供规则描述及告警修复指导

——检查结果有优先级/严重程度的划分，能跟踪到状态

——支持检查规则配置，支持单个告警/批量告警/告警路径屏蔽等功能

——自动生成代码检查报告，有新增/修复/遗留告警等质量度量指标

——多种工具检查结果能够整合展示在报告中便于开发团队修复

##### 可以包含以下高级功能：

——能够开展增量代码扫描，自动识别问题引入者

——能够集成进IDE中在编码更前端开展检查

——根据项目实际场景支持检查规则定制

——支持和缺陷管理系统打通，具备跟踪和驱动修复的能力

——代码检查报告中自动生成新增/修复/遗留告警趋势量化展示项目代码质量状态

——代码检查工具支持集成到持续交付流水线中自动运行实施

——支持配置项目代码质量符合度标准，在流水线中自动化实施，作为下一个环节的准入条件

### 2. 单元测试

单元测试是项目的开发质量管理活动。单元测试具备自动化、独立性、可重复执行的特点。


##### 应包含以下基本功能：


——每个CASE有assert 来验证

——单元测试的CASE有手工编写和自动化生成2种，文件名要区分

——每个单元测试CASE执行时间不超过1秒,可以指定超时时间。

——单元测试的报告中必须有分支覆盖率，CASE总数，成功执行总数，失败总数，异常总数，执行跳过总数

——单元测试和源代码用目录结构区分开

——使用单元测试框架

——支持排除目录文件

——单元测试支持修改记录

——单元测试支持评审记录，和源代码评审保持一致。



##### 可以包含以下高级功能：

——使用MOCK

——单元测试的参数范围支持开发和测试提供的数据范围

——使用工具自动化生成单元测试

——单元测试支持并行运行

——单元测试数据支持来自NLP分析得到的数据

### 3. 接口/服务测试

接口测试是通过直接在消息层向测试软件接口，确定功能、性能、可靠性、安全等是否满足预期的软件测试方法。REST风格接口是Web应用前后端和微服务之间主要的接口形式。

##### 应包含以下基本功能：

——支持针对REST风格接口的测试

——支持HTTP、HTTPS协议GET、POST、PUT、DELETE等主要方法的测试

——支持基于Swagger或Open API文档辅助编写接口测试逻辑（建议放到高级）

——支持基于录制的接口请求和响应生成测试逻辑（建议放到高级）

——支持定义HTTP请求的URL、请求头、请求报文

——支持表单、文本、JSON、XML等多种格式的请求报文

——支持Basic认证、Token认证等接口鉴权认证方式

——支持针对HTTP响应的响应报文、响应头、响应码定义测试断言

——支持提取HTTP响应的内容，基于上下文创建后续HTTP请求

——支持循环、判断、暂停等测试逻辑 （建议描述为接口测试流程控制）

——支持定义不同测试环境的测试参数

——支持测试关键字，以复用测试逻辑（术语中增加关键字驱动，复用测试逻辑建议作为单独特性）

——支持测试套件编排测试用例串行顺序执行或并行执行（可能不是接口测试专有特性）

——支持调试测试用例，以验证测试逻辑（可能不是接口测试专有特性）

——支持记录测试执行日志和结果（可能不是接口测试专有特性）

——支持定义接口Mock，以解耦开发和测试依赖（目的建议去掉）

——支持流水线调用接口测试实现持续集成和持续测试

——支持接口测试覆盖率和测试通过率统计

专家评审：
1、rest风格描述过细，其它接口测试没有提到；

##### 可以包含以下高级功能：

——xxxx

——xxxx

### 4. UI测试

UI测试是用户界面测试，英文名为User interface testing的简称。它通过浏览测试对象可正确反映业务的功能和需求，这种浏览包括窗口与窗口之间、字段与字段之间的浏览，以及各种访问方法 （Tab 键、鼠标移动和快捷键）的使用，且窗口的对象和特征都符合需求。

##### 应包含以下基本功能：

——在实际运行环境或模拟器中打开被测对象

——模拟用户通过键盘、鼠标等进行的人机交互操作

——被测对象的内容和属性的检查

——测试步骤局部修改

——测试过程用例管理

——测试过程的本地回放、执行

##### 可以包含以下高级功能：

可以包含以下高级功能：

——测试过程局部调试

——自动录制测试过程

——参数化测试过程中相应数据

——被测对象相应内容（文案、数值等）支持数据库对比

——重复过程的公共方法

——支持一套脚本在不同环境(如本地开发环境、云端测试环境等)中执行

——支持对云端执行的测试任务的管理

——定时执行

### 5. 移动应用测试

移动应用测试是指针对市场主流移动端（Android、iOS、H5、小程序等）利用自动化技术进行功能性和各项非功能性专项测试。包含适配兼容测试、移动自动化测试、客户端性能测试三大类测试。

#####适配兼容测试 

适配兼容测试利用移动终端真机实验室，移动应用需要在各种参数搭配的机型上进行测试,以确保移动应用兼容用户使用的手机机型, 最大化客户群体。

##### 应包含以下基本功能

——按需的机型选择
a)Android/iOS操作系统版本
b)主流厂商的定制ROM
c)屏幕分辨率
d)硬件配置（CPU、GPU、内存）
e)市场Top用户占比机型
f)支持自选机型
针对H5
g)各大厂商的浏览器和内核
h)WebView（如微信）

——安装、拉起、Monkey遍历、卸载

——适配问题的检测能力（崩溃、无响应、安装失败、拉起失败、卸载失败、UI异常、Exception）

——测试执行步骤的还原（操作和截图）

——基础性能指标采样（安装时间、启动时间、CPU、内存、流量、FPS）

——系统日志的收集

##### 可以包含以下高级功能：

——用户账户自动登录

——支持运行主流自动化框架（如Appium、UIAutomator、XCTest）和自定义框架编写的兼容测试脚本（主流自动化框架，建议举例或修改描述，安卓官方、或苹果官方？此处是否体现自定义框架？已修改）

——支持自定义日志上报和导出

——支持API接口提交任务和接口文档

——能够对出现具体问题的设备进行远程调试

##### 移动自动化测试：

移动自动化测试，英文名为Mobile Test Automation的简称，它是将移动应用作为测试对象，把以人为驱动的测试行为转化为机器执行的一种过程。通常，在设计与编写用例脚本后，由测试人员上传至移动终端真机实验室自动执行测试，得到实际结果与期望结果的对比评估。在此过程中，达到节省人力、时间或硬件资源，增强测试深度，提高测试效率等效果。

##### 应包含以下基本功能

——支持通用的自动化测试框架 

——模拟用户对应用的操作（点击、滑动、长按、轨迹操作、文本输入等）

——基本的识别能力（标准控件识别）

——测试信息管理能力（用例、日志、缺陷、报告）

——移动设备的管理运维能力（故障等重连、重测机制，设备稳定性）

##### 可以包含以下高级功能：

——支持用户修改过的开源框架

——提供插件集成到开发IDE中

——提供丰富的Open API（包含设备信息获取，筛选，提测，结果拉取等灵活，详细的API能力）

——在云端设备上进行脚本调试

——进阶的识别能力（OCR识别，UI识别，游戏引擎层控件识别等）

——脚本录制及精准回放能力

——任务运行可视化及灵活干预能力（以单台设备为粒度进行终止、重测等干预操作）

——性能数据采集调试能力（包含FPS、内存等通用性能，以及引擎层的性能）

——云端设备灵活配置和高效调度能力

##### 客户端性能测试：
客户端性能测试利用移动终端真机实验室，通过在不同参数搭配的各档机型上利用性能测试工具获得各项性能指标，定位性能瓶颈和问题根本原因，提升移动应用的性能表现，以保障用户获得流畅、稳定的最佳使用体验。

##### 应包含以下基本功能
  
——机型性能天梯（机型分档）

——基础性能指标采样（安装时间、首屏时间、响应时间（启动、滑动、界面切换等）、CPU、内存、流量、FPS、耗电量、温度、IO)-客户端必要的指标

——测试执行步骤的还原（操作和截图）

——系统日志的收集

——测试报告的导出

##### 可以包含以下高级功能：

——支持运行主流自动化框架（如Appium、UIAutomator、XCTest）和自定义框架获取性能数据（跟前面的主流自动化框架描述问题一样已修改）

——支持版本对比、竞品对比

——支持API接口批量获取性能数据

——过度绘制检测

——支持性能问题根因分析

——支持多性能指标组合分析（建议高级增加 支持性能指标组合分析已添加）

——针对游戏提供unity3d,unreal 4引擎的深度性能数据

——针对H5提供瀑布流视图，连接视图，提供实时抓包、修改功能
 
专家评审：
1、建议高级增加 支持性能指标组合分析


### 6. 性能测试

性能测试xxxx。

##### 应包含以下基本功能：

——支持性能测试项目的测试脚本、测试结果、测试报告的基本管理功能；

——支持主流测试协议；

——支持负载参数集读取数据文件功能；

——支持负载参数集自动生成序列数字、随机数字等功能；

——负载参数集数据读取支持：顺序、随机、数据文件读取、数据文件分段读取、文件读取的功能； 

——支持脚本逻辑控制功能，脚本编辑功能；

——支持性能测试结果数据输出，包括测试发送数据及服务端响应数据等；

——支持思考时间设置功能；

——支持请求超时、响应超时设置功能；

——支持性能测试执行过程中服务端回送数据正确性检查的功能；

——支持长连接、短连接设置；

——支持数据上下文关联的功能；	

——支持性能测试场景设置功能，性能场景：性能测试过程中模拟真实用户的服务流程或业务处理过程的一系列动作的集合；

——支持性能测试指标数据实时输出的功能；

——支持性能测试报告查看及导出功能；

——支持采集性能监控指标的功能；

——支持性能测试过程中各类错误显示、汇聚的功能；

——HTTP、HTTPS协议应支持GET、POST方法的测试；

——支持HTTP协议COOKIE设置；

##### 可以包含以下高级功能：

——当分布式压力源未用尽时，系统支持多个测试用户同时调用压力源发起性能测试直到压力资源满载；

——支持多种协议的性能测试； 

——支持自定义协议的性能测试；

——支持测试数据集可通过脚本或程序灵活生成；

——支持从数据库中自动读取负载参数集的功能；
（这类需求的适用场景相对狭窄，且产品自研的实现成本非常高，我们对它是否需要写进一个国家标准存疑）

——支持灵活配置、快速扩充压力源的功能；

——支持测试节点调用互联网公有云资源、局域网私有云资源、或其它可用的虚拟及物理资源；

——支持相同测试场景执行报告比对功能；

——支持采集各种性能指标的功能，如：网络通信指标、中间件指标、数据库指标等；

（如果全部都要采集实现成本非常高，且系统本身已经有替代功能。是否有必要写进国标？

如果坚持要写，那么希望可以列清楚需要具体需要采集哪些）

——支持可配置的性能测试挡板。性能测试挡板：在跨系统测试中由于客观原因等无法模拟全部测试流程中的非主要测试系统资源，故通过软件或程序来模拟其他相关系统的操作，该软件或程序称之为挡板，主要目的是保证测试流程的完整性；（希望可以把“挡板”的解释放进“术语定义”章节）

——支持集成外部工具进行性能分析；（是进行“性能测试”还是“性能分析”？如果是性能分析，主要是指哪个层面？）

——HTTP、HTTPS高级功能支持OPTIONS、HEAD、PUT、DELETE、TRACE、CONNECT方法的测试；(从经验来看，用户较少用这些方法，是否需要都加上？用户基本用不上，且实现这个功能没什么技术难度，对于产品来说，这个应该算不上加分项。）

——HTTP、HTTPS、Socket协议支持脚本自动化录制、回放功能；（加列了socket协议的原因是？如果加上socket，那TCP、PB的录制是否也需要加上？）
