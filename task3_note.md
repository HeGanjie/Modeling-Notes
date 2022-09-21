# task_03 回归分析2_线性回归模型的推断与推广

[教程地址](https://github.com/Git-Model/Modeling-Universe/blob/main/Data%20Analysis%20and%20Statistical%20Modeling/task_03%20%E5%9B%9E%E5%BD%92%E5%88%86%E6%9E%902_%E7%BA%BF%E6%80%A7%E5%9B%9E%E5%BD%92%E6%A8%A1%E5%9E%8B%E7%9A%84%E6%8E%A8%E6%96%AD%E4%B8%8E%E6%8E%A8%E5%B9%BF/%E5%9B%9E%E5%BD%922.ipynb)

# 简单总结
3. 回归分析的重要任务——推断/假设检验
  * 需要借助概率论与数理统计中假设检验的知识来辨别：一个系数怎样子才算是接近0（影响不显著）
  * t检验
    * 是回归分析中单个线性假设检验问题的常用检验方法
    * 从单参数检验：若 |beta - C| > 0 则说明参数 beta 影响显著
    * 显著性水平：alpha = P(|无偏beta| > C)
    * 实际计算时先计算$\frac{\hat{\beta}_{j}-\beta_{j}}{\operatorname{se}\left(\hat{\beta}_{j}\right)}$，再与python输出的t分布对应的双侧分位点值$\pm {t_{n-k-1}\left( 1-\frac{\alpha}{2} \right)} $进行比较 （双边检验）
  * 单边检验：
    * 用于判断某某自变量对因变量是否存在正效应影响  
