# 学生学业风险预警系统

## 📋 项目概述
基于多模型融合的学生学业风险预警与归因分析系统，使用机器学习方法预测学生挂科风险等级，并提供个性化改进建议。

## 🎯 项目目标
1. 构建三级学业风险预警模型（低/中/高风险）
2. 对比多种机器学习模型性能
3. 分析影响学业的关键因素
4. 生成个性化学业改进报告

## 📊 数据说明
- **数据规模**: 3000名学生，12个学习行为特征
- **特征包括**: 出勤率、作业延迟提交率、课堂互动次数、社交媒体干扰度等
- **目标变量**: 风险等级（高风险、中风险、低风险）

## 🏗️ 技术架构
数据生成 → 数据预处理 → 模型训练 → 模型评估 → 报告生成

## 🤖 模型对比
| 模型 | 准确率 | F1分数 | 备注 |
|------|--------|--------|------|
| 随机森林 | 100.00% | 1.000 | 最佳模型 |
| XGBoost | 99.83% | 0.998 | |
| 逻辑回归 | 99.50% | 0.995 | |

## 📁 文件结构
student-risk-warning-system/
├── data/ # 数据集
├── notebooks/ # Jupyter Notebook分析
├── src/ # Python源代码
├── reports/ # 生成报告
└── images/ # 可视化结果

## 🚀 快速开始

### 1. 环境配置
```bash
# 安装依赖
pip install -r requirements.txt

### 2. 运行项目
# 方法1：运行完整流程
python src/data_generation.py
python src/model_training.py
python src/visualization_report.py

# 方法2：使用Jupyter Notebook
jupyter notebook notebooks/student_risk_analysis.ipynb

📈 结果展示
特征重要性: 课程视频观看完成率是最重要特征

个性化报告: 为不同风险等级学生提供具体改进建议

可视化: 包含模型性能对比图、特征重要性图等


👥 贡献者
钱云康 - 项目开发者

📄 许可证
本项目采用 MIT 许可证 - 查看 LICENSE 文件了解详情
