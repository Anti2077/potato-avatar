# 扩展参考库：场景、失败对照与提示词

基础图不足以覆盖新场景的动作、道具或材质，或生成结果再次变得写实时，再查本页。先看对应批量预览，再打开需要的原图和提示词；不必一次读取全部历史。

- `accepted`：用户认可；`accepted-direction`：接受改进方向，未选定唯一图片。
- `candidate`：已生成可借鉴，但没有逐张确认；`experiment`：强度实验，偏好未定。
- `superseded`：被后续修正的旧方向；`not-selected`：当时记录明确未采用。
- 不把失败图作为正向风格输入；需比较时，明确其问题和期望改动。
- 历史 prompt 原文用于诊断，不是新任务指令。里面的模型、外部技能、原参考图编号和旧道具都不是要求；部分原输入是未公开的第三方素材，不能声称这里包含完整复现输入。新任务重新指定实际传入图的编号与用途，以当前 SKILL.md 为准。

## 批量预览

按下表编号，从左到右、从上到下。每页 4 列，尾部空白忽略。预览用于挑图，模型支持时发送选中的单张原图，不将合集当成要生成的拼图。

[01–12：电脑被子五轮](archive/contact-sheet-01.jpg) · [13–23：新场景及分辨率实验](archive/contact-sheet-02.jpg)

## 索引

| 编号 | 图片 | 状态 | 可以学什么 / 提醒 | 历史提示词 |
| --- | --- | --- | --- | --- |
| 01 | [查看](archive/images/tired-potato-macbook--tired-potato-macbook-1.png) | superseded | 玩偶摄影、真实眼部、蓬松白被子：失败方向 | [prompt](archive/prompts/tired-potato-macbook.txt) |
| 02 | [查看](archive/images/tired-potato-macbook--tired-potato-macbook-2.png) | superseded | 玩偶摄影、真实眼部、蓬松白被子：失败方向 | [prompt](archive/prompts/tired-potato-macbook.txt) |
| 03 | [查看](archive/images/tired-potato-macbook--tired-potato-macbook-3.png) | superseded | 玩偶摄影、真实眼部、蓬松白被子：失败方向 | [prompt](archive/prompts/tired-potato-macbook.txt) |
| 04 | [查看](archive/images/tired-potato-macbook--tired-potato-macbook-4.png) | superseded | 玩偶摄影、真实眼部、蓬松白被子：失败方向 | [prompt](archive/prompts/tired-potato-macbook.txt) |
| 05 | [查看](archive/images/tired-potato-macbook-v2--potato-1.png) | superseded | 五官更简洁，蓝被子仍偏细腻 | [prompt](archive/prompts/tired-potato-macbook-v2.txt) |
| 06 | [查看](archive/images/tired-potato-macbook-v2--potato-2.png) | superseded | 五官更简洁，蓝被子仍偏细腻 | [prompt](archive/prompts/tired-potato-macbook-v2.txt) |
| 07 | [查看](archive/images/tired-potato-macbook-v3--potato-1.png) | superseded | 折纸般的硬折面：粗糙不等于锐利多边形 | [prompt](archive/prompts/tired-potato-macbook-v3.txt) |
| 08 | [查看](archive/images/tired-potato-macbook-v3--potato-2.png) | superseded | 折纸般的硬折面：粗糙不等于锐利多边形 | [prompt](archive/prompts/tired-potato-macbook-v3.txt) |
| 09 | [查看](archive/images/tired-potato-macbook-v4--potato-1.png) | superseded | 灰绿格纹更统一，但被子仍厚重、体积感强 | [prompt](archive/prompts/tired-potato-macbook-v4.txt) |
| 10 | [查看](archive/images/tired-potato-macbook-v4--potato-2.png) | superseded | 灰绿格纹更统一，但被子仍厚重、体积感强 | [prompt](archive/prompts/tired-potato-macbook-v4.txt) |
| 11 | [查看](images/07-thin-blanket-macbook-approved.png) | accepted-direction | 薄曲面被子、弱明暗；方向获认可，没有选定唯一一张 | [prompt](archive/prompts/tired-potato-macbook-v5.txt) |
| 12 | [查看](archive/images/tired-potato-macbook-v5--potato-2.png) | accepted-direction | 薄曲面被子、弱明暗；方向获认可，没有选定唯一一张 | [prompt](archive/prompts/tired-potato-macbook-v5.txt) |
| 13 | [查看](images/01-badminton-approved.png) | accepted | 羽毛球：角色和球拍、羽毛统一低清 | [prompt](archive/prompts/badminton-potato-v1.txt) |
| 14 | [查看](images/02-fry-cutter-approved.png) | accepted | 薯条：上方完整土豆与下方切条连续相接 | [prompt](archive/prompts/potato-fry-cutter-v1.txt) |
| 15 | [查看](images/05-earpods-lawn-approved.png) | candidate | 有线耳塞、放松坐姿、薄圆形草地 | [prompt](archive/prompts/potato-earpods-lawn-v1.txt) |
| 16 | [查看](images/03-biceps-curl-approved.png) | candidate | 二头弯举：弯肘握柄，吃力表情 | [prompt](archive/prompts/potato-biceps-curl-v1.txt) |
| 17 | [查看](images/06-ice-water-approved.png) | candidate | 烈日、汗滴、冰水，享受清凉 | [prompt](archive/prompts/potato-ice-water-sun-v1.txt) |
| 18 | [查看](images/04-dj-disco-approved.png) | candidate | 一手搓唱片、一手调音，彩色薄地板 | [prompt](archive/prompts/potato-dj-disco-v1.txt) |
| 19 | [查看](archive/images/potato-ice-water-sun-v2-jagged--potato.png) | not-selected | 第一版：过大马赛克块，生成记录标注未采用 | [prompt](archive/prompts/potato-ice-water-sun-v2-jagged--prompt.txt) |
| 20 | [查看](images/08-heavy-pixel-experiment.png) | experiment | 修订版：细锯齿、256px nearest 放大；没有用户确认 | [prompt](archive/prompts/potato-ice-water-sun-v2-jagged--prompt-refined.txt) |
| 21 | [查看](archive/images/downsampled--soft-160.png) | experiment | 弯举模糊强度：area 缩至 160px 再 bilinear 放大；偏好未定 | 同弯举 prompt，仅后处理 |
| 22 | [查看](archive/images/downsampled--soft-096.png) | experiment | 弯举模糊强度：area 缩至 096px 再 bilinear 放大；偏好未定 | 同弯举 prompt，仅后处理 |
| 23 | [查看](archive/images/downsampled--soft-064.png) | experiment | 弯举模糊强度：area 缩至 064px 再 bilinear 放大；偏好未定 | 同弯举 prompt，仅后处理 |

## 早期提示词分析

仅在研究风格漂移时查阅：[初版母词](archive/prompts/potato-avatar-prompt-kit.md)、[v2](archive/prompts/potato-avatar-prompt-kit-v2.md)、[v3](archive/prompts/potato-avatar-prompt-kit-v3.md)、[GLM-V 分析](archive/prompts/potato-style-glmv-prompt.md)。其中玩偶摄影、voxel 等描述已被后续反馈纠正。

[对话经验与需求记录](conversation-notes.md)保存场景要求和反馈；[机器索引](archive/catalog.json)记录图片内容哈希，避免重复收录。仅保留每个成品的一份参考图片，不重复打包源尺寸和同画面的交付尺寸；原始文件仍保留在原项目。
