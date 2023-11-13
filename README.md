# DataWahle--
2023全球智能汽车AI挑战赛（赛道二：视频数据理解赛道）的学习记录

Baseline思路是：使用了OpenAI的预测训练模型Clip(图像和文本进行联合编码计算相似性进而匹配实现多模态)进行视频到文本的对应结构抽取，抽取第一帧的图像直接暴力使用Clip进行匹配后选择概率最大的进行输出
![image](https://github.com/KillerWS/DW_Nov/assets/39308981/ad02fd1b-2cf8-4f3f-8da4-5ba138fd8228)

可以尝试的优化方向：
数据源增强：考虑时序多帧处理思路
微调Clip模型：替换最后一层（可选）：指定新任务的类别以适应微调任务。
To do...

References & Resource
CLIP: https://openai.com/blog/clip/
预训练模型: https://huggingface.co/models
