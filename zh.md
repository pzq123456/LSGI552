# Project proposal : Geo-Info Agent for LLM in Browser

## Abstract

本项目旨在开发一个运行于浏览器的代理框架，专门为大语言模型（LLM）设计，以增强其对地理数据的理解和处理能力。该框架将通过提供空间分析接口和动态生成地理信息描述的能力，帮助 LLM 在特定空间上下文中提供更加精准的回答。

## Research Questions & Methodology
1. 代理框架如何确保结果的准确性（尤其是关于空间位置关系）？
   - 代理框架将通过 JavaScript 实现关键的空间分析和位置关系计算，确保数据处理的精确性。通过将复杂的空间关系转化为结构化的语言描述，能够减少 LLM 生成模糊或不准确答案的几率。JavaScript 作为浏览器内运行的主流编程语言，能够无缝集成到浏览器的执行环境中，直接验证和优化模型的输出。
2. 如何将地图中的信息传达给大语言模型？
   - 代理框架将基于用户当前的地图视图状态（如视窗中心、缩放级别等），结合上下文中的关键词，有针对性地生成地理描述。描述将包括方位、距离、地标等信息，以确保 LLM 能够准确理解用户的空间环境和需求，并生成具有空间相关性的回答。
3. 框架的拓展性？
   - 框架将通过模块化的设计，允许开发者创建和扩展功能组。这些功能组将包含不同类型的空间数据处理接口，如坐标转换、空间关系计算、路径分析等，从而使得框架具有高度的扩展性，适应各种地理信息应用场景。
4. 错误处理？
   - 框架将提供代码预览和编辑功能，当 LLM 生成空间分析函数时，用户可以预先查看并确认代码片段。在确认后，代码将在 Web Worker 中运行，以避免阻塞主线程，并提升系统的稳定性。任何错误都将通过日志和用户提示进行处理，确保及时纠正问题。

Hello,

I plan to work on a project titled "Geo-Info Agent for LLM in Browser". The goal is to create a browser-based framework that enhances large language models' ability to understand and process geographic data.

Best regards,
Zhiqing Pan