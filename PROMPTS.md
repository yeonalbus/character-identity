# 测试集与对应提示词

## lora与lbw配置

strength_model：1.00
strength_clip：1.00

self_attn：1.0
cross_attn：0.7
mlp：0.7
层间权重：
```
0.3,0.3,0.3,0.3,0.3,0.3,0.3,0.3,0.8,0.8,0.8,0.8,0.8,0.8,1.0,1.0,1.0,1.0,1.0,0.8,0.8,0.8,0.8,0.0,0.0,0.0,0.0,0.0
```

## 通用的提示词

质量词
```
very aesthetic, masterpiece, best quality, good quality, 
highres, absurdres, year 2025, score_9, score_8, score_7,
```

人数
```
1girl,
```

动作
```
standing, contrapposto, looking at viewer, slight smile,
```

场景
```
simple background, white background,cowboy shot,
A cowboy shot of a girl standing in a contrapposto pose, looking at the viewer with a slight smile, against a simple white background.
```

## 角色提示词（便于后续进行替换）

角色基本触发词
```
gin ran \(megami device\)
```

身材（非头部角色本体）
```
lolicon,curvy,large breasts,
```

头部角色本体
```
发型：long hair,streaked hair,orange eyes,
发色：white hair,black hair,two-tone hair,
```

头饰（头部穿戴物）
```
animal ears,mechanical ears,white headwear,hair ornament,hair bow,white ornament,
```

服装（非头部穿戴物）
```
white bra,metal bra,black bow,purple bow,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
```

配饰（非头部穿戴物）
```
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```
## 需要替换的提示词

基线
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
long hair,white hair,black hair,two-tone hair,streaked hair,orange eyes,
animal ears,mechanical ears,white headwear,hair ornament,
white bra,metal bra,black bow,purple bow,hair bow,white ornament,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```

单剥头饰
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
long hair,white hair,black hair,two-tone hair,streaked hair,orange eyes,

white bra,metal bra,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```

单剥眼型
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
long hair,white hair,black hair,two-tone hair,streaked hair,orange eyes,
(round eyes:6),
animal ears,mechanical ears,white headwear,hair ornament,
white bra,metal bra,black bow,purple bow,hair bow,white ornament,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```

单剥发型
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
orange eyes,white hair,black hair,two-tone hair,
twin tails,
animal ears,mechanical ears,white headwear,hair ornament,
white bra,metal bra,black bow,purple bow,hair bow,white ornament,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```

单剥发色
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
orange eyes,long hair,streaked hair,
(golden hair:4),(brown hair:2),
animal ears,mechanical ears,white headwear,hair ornament,
white bra,metal bra,black bow,purple bow,hair bow,white ornament,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```

剥头饰+眼型
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
long hair,white hair,black hair,two-tone hair,streaked hair,orange eyes,
(round eyes:6),

white bra,metal bra,black bow,purple bow,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```

剥头饰+发型
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
orange eyes,white hair,black hair,
twin tails,

white bra,metal bra,black bow,purple bow,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```

剥眼型+发型
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
orange eyes,white hair,black hair,two-tone hair,
(round eyes:6),(twin tails:4),
animal ears,mechanical ears,white headwear,hair ornament,
white bra,metal bra,black bow,purple bow,hair bow,white ornament,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```

三剥
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
orange eyes,white hair,black hair,two-tone hair,
(round eyes),(twin tails),

white bra,metal bra,black bow,purple bow,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,

负面提示词：animal ears,mechanical ears,white headwear,hair ornament,
```

单剥服装
strength_model：0.90
```
gin ran \(megami device\), lolicon, curvy, large breasts, long hair, white hair, black hair, two-tone hair, streaked hair, orange eyes, animal ears, mechanical ears, white headwear, hair ornament, miko, 
```

单剥配色
```
gin ran \(megami device\),
lolicon,curvy,large breasts,
long hair,white hair,black hair,two-tone hair,streaked hair,orange eyes,
animal ears,mechanical ears,white headwear,hair ornament,
white bra,metal bra,black bow,purple bow,hair bow,white ornament,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,

(暂时不清楚怎么剥离，因此此测试没有实施)
```

单剥本体
```
gin ran \(megami device\),
(milf:2),(mature female:2),(flat chest:2),
long hair,white hair,black hair,two-tone hair,streaked hair,orange eyes,
animal ears,mechanical ears,white headwear,hair ornament,
white bra,metal bra,black bow,purple bow,hair bow,white ornament,skirt,underboob,bare shoulders,thighs,bare legs,pale skin,underwear,
yellow thigh strap,high heels,
black arm warmers,purple arm warmers,black gloves,claw glove,
```

全剥离
```
(twin tails:2), brown hair, black eyes,
round eyes, looking at viewer, slight smile,
milf, mature female, flat chest,
simple white dress, simple background, white background,
standing, contrapposto, cowboy shot,
```

~~干扰图~~
```
插一张与银狼长得像的
```

**不设干扰图（删除原 # 14）的理由：**

1. **误认的发生条件**。按本理论（观点一、六），假唤醒需要三个条件同时成立：观察者对目标角色有先验、对干扰角色无先验（干扰角色不进入候选集）、且干扰角色与目标角色共享足够特征，使其特征组合在候选集内构成唯一匹配。
2. **本实验的观察者均按"先验人群"选取**（方法论 2），即认识银狼者。若干扰图选用观察者认识的角色，则候选集内存在竞争者、唯一性不成立，结果是不确定而非误认——干扰图只能得到预期内的"否"，不提供关于假唤醒的信息；若干扰图选用观察者不认识的角色，则无法保证"不认识"（观察者池与干扰角色集合不可控），该条件无法稳定构造，且"认识 A、不认识 B"的观察者需要独立的筛选环节。
3. **不在本实验的分析目标内**。本实验测的是层归属、层内强度、跨层交互；特异性/假唤醒属于"候选集密闭条件"下的另一维度检验，应以独立的"无先验对照组"设计，不宜与本实验合并。
4. **资源约束**。二游设计中"特征完整、与目标高度相似、且能被观察者稳定地认定为'不认识'的角色"本身稀缺，找图与配对成本高。
