# Reason Model 交互平台

基于 Streamlit 构建的多功能 AI 对话应用，支持API调用、文件分析、网络搜索和对话历史管理。

## 主要功能

- 文件分析：支持上传并分析 PDF、Word、TXT、CSV 等格式文件
- 网络搜索：支持文本、新闻、图片、视频等多种搜索模式
- 图片理解：支持上传图片进行多模态对话（仅支持多模态模型）
- 对话历史：支持保存和加载历史对话记录
- 用户系统：支持用户注册和登录
- 参数配置：支持自定义 Temperature、Top P 等模型参数
- 实时对话：支持流式输出对话内容

### 快速开始
 - pip install -r requirements.txt
 - 配置API_key
 - streamlit run main.py