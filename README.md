# Streamlit拼好网

这是一个基于Streamlit开发的多功能Web应用平台，集成了多种AI和工具功能。

~~具体套百家壳还差91家~~

## 🌟 主要功能

### AI交互模块
- **AI对话平台**：支持多模态交互、参数调整、文件上传、网络搜索等功能
- **文本生成图像**：基于AI的图像生成功能

### Dify工作流
- **小红书文案生成**：智能生成符合小红书平台风格的文案内容

### 实用工具集
- **知识图谱检索**：基于知识图谱的RAG工具
- **PDF固版翻译**：保持原PDF排版格式的翻译工具
- **分割万物**：基于SAM2.1的语义分割工具
- **论文分段润色**：学术论文智能润色工具
- **天眸预警**：天气实时预警工具

## 🚀 快速开始

### 环境要求
- Python 3.11

### 安装步骤

1. 克隆项目并安装依赖：
```bash
git clone https://github.com/Tian-ye1214/StreamlitKit.git
pip install -r requirements.txt
```

2. 配置环境变量：
- 在项目根目录创建`.env`文件
- 配置必要的API密钥

3. 下载必要模型：
- DocLayout模型：下载`doclayout_yolo_docstructbench_imgsz1024`模型并放入`pages/ModelCheckpoint`目录
  - 下载地址：https://huggingface.co/wybxc/DocLayout-YOLO-DocStructBench-onnx/tree/main
- SAM2.1模型：下载并放入`pages/SAM2_1/checkpoints`目录
  - 下载地址：https://github.com/facebookresearch/sam2
- GroundingDINO模型：下载并放入`pages/ModelCheckpoint/GroundingDINO-T`目录
  - 下载地址：https://huggingface.co/IDEA-Research/grounding-dino-tiny/tree/main

4. 启动应用：
```bash
streamlit run main.py
```

## 📦 项目结构
```
.
├── main.py              # 主程序入口
├── requirements.txt     # 项目依赖
├── .env                # 环境变量配置
├── navigation/         # 导航模块
├── pages/             # 功能页面
│   ├── ModelCheckpoint/  # 模型检查点
│   └── SAM2_1/          # SAM2.1模型
└── user_logs/         # 用户日志
```

## 🔧 技术栈
- Streamlit：Web应用框架
- OpenAI：AI模型接口
- PyMuPDF：PDF处理
- LightRAG：知识图谱构建
- SAM2：语义分割
- 其他依赖见requirements.txt

## 🙏 致谢
感谢以下作者对代码的贡献：
- [@mwx66](https://github.com/mwx66)
- [@yanyunxi](https://github.com/yanyunxi)

