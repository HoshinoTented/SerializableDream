# Buffs 增幅

增幅分为正面增幅（Buff）和负面增幅（Debuff）。

基础的正面增幅有：

* 自愈(h)：回复 $h 点生命值
* 灵之触(h)：回复 $h 点心智
* 无棱星(h, d)：受到伤害时，最多减免 $d 点伤害，无棱星具有 $h 点生命值

等

基础的负面增幅有：

* 魔力侵蚀(d)：魔力侵蚀状态下，每回合受到 $d 点魔法伤害，并且该单位每消耗魔力时，对其造成 $d * (消耗魔力（最大为该单位的魔力储能的 36%） / 6) 点伤害，并且该单位受到的魔法伤害提高 10%
* 污血溪(d)：污血溪状态下，每回合受到 $d 点魔法伤害，并且该单位受到物理伤害时，将获得 污血溪($d * 2) 效果
* 噩梦之井(d)：噩梦之井状态下，每回合损失 $d 点心智，并提高黑色噩梦系技能 82% 的全伤害