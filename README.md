# dehaze
---
Realizing Kaiming He's paper 'Single Image Haze Removal Using Dark Channel Prior'

- 雾霾天应当是白天（晚上关了灯还去什么雾），因此在计算大气光时，我假设最亮部分是灰白色（先验！雾霾天我见得多了！），那R/G/B应该都很接近255，so没必要分开算RGB，具体见代码
- When I calculate the A(atmosphere), I simply suppose the brightest spot is approximately white. So the RGB value of that point should be almost same
- 使用导向滤波精确透光率
- Using the guided filter now.
