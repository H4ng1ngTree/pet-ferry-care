# data 占位说明

这里放数据新闻项目的原始数据和清洗后数据。

建议目录：

```text
data/
├── raw/        # 原始数据，例如问卷导出、企查查/天眼查截图整理、政策文件表
└── processed/  # 清洗后的 CSV/JSON，用于制图
```

建议至少保留这些表：

| 文件名 | 内容 |
| --- | --- |
| survey_pet_funeral.csv | 团队问卷数据，样本量 n=57 |
| company_growth.csv | 相关企业年度存量和新增注册数量 |
| company_region.csv | 相关企业地区分布 |
| policy_timeline.csv | 政策、政府答复、团体标准时间线 |
| worker_profiles.csv | 从业者案例、年龄、城市、入行动机、过往职业 |
| industry_problems.csv | 行业乱象分类与案例来源 |
