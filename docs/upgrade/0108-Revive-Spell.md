---
title: "部落冲突 coc 复苏法术（复活法术）升级数据"
navTitle: "复苏法术"
shownTitle: "复苏法术（复活法术）"
description: "天使的独家秘方！复苏法术能让效果范围内被击倒的英雄恢复一部分生命值，重新回到战斗中。将该法术带入战斗，被击倒且可复苏的英雄上方就会出现一颗漂浮的金色心脏。升级复苏法术，可为英雄恢复更多生命值。"
module: upgrade-home
imgFolder: home_tech/0108
wiki: https://clashofclans.fandom.com/wiki/Revive_Spell
canonical: /upgrade/0108-Revive-Spell
---

<UnitInfo :folder="$frontmatter.imgFolder" imgSrc="Revive_Spell_info.png" :imgAlt="$frontmatter.navTitle" :description="$frontmatter.description" />

<SmallTitle>重要说明</SmallTitle>

1. 复苏法术仅在英雄被击倒时有效。如果玩家还有未使用的复苏法术，则被击倒的英雄上方会出现一颗漂浮的金色心脏，表示它们可以重新加入战斗。使用复苏法术后，法术会瞄准有效范围内最近的英雄并复苏，使其恢复大部分生命值。
    - 如果法术有效范围内没有符合条件的英雄，则法术不会生效，会直接浪费掉。
    - 如果法术有效范围内有多个符合条件的英雄，则只对距离法术部署位置最近的英雄有效。
2. 复苏法术可以对同一英雄使用多次。
3. 只有当英雄的自动技能和 [凤凰](/upgrade/0287-Phoenix) 的无敌效果都结束后，你才能对被击倒的英雄使用复苏法术。
    - 英雄的自动技能指的是设置中的“即将被击败时自动使用技能”选项，这个选项默认打开。
5. 如果英雄在使用技能时被击倒，复苏后剩余的技能时间还在。
6. 如果带有战宠的英雄被击倒，则英雄在第一次被击倒时就会与宠物分离，复苏后英雄和宠物互不影响。

<SmallTitle>属性</SmallTitle>

<UnitProperties>
    <UnitProperty pKey="有效半径" pValue="8 格" />
    <UnitProperty pKey="作用类型" pValue="复活英雄" />
    <UnitProperty pKey="作用目标" pValue="我方英雄" />
    <UnitProperty pKey="占用的法术空间" pValue="2" />
    <UnitProperty pKey="所需法术工厂等级" pValue="8" />
    <UnitProperty pKey="所需大本等级" pValue="15" />
    <UnitProperty pKey="法术配置时间" pValue="360" trainingSystem="2022" />
</UnitProperties>

<SmallTitle>升级数据</SmallTitle>

<script setup>
const tableExtraInfo = [
    {
        "column": 2,
        "type": "cost",
        "gpClass": "research",
        "icon": "Elixir"
    },
    {
        "column": 3,
        "type": "time",
        "gpClass": "research"
    }
];
</script>

<UnitTable :tableExtraInfo="tableExtraInfo">

| 等级 |复苏后<br>回复的血量| 升级花费 |  升级时间  |所需<br>实验室等级|所需<br>大本等级|
| ---- |        ---       |    ---   |    ---    |       ----      |      ----    |
|   1  |        60%       |     \    |      \    |         1       |       15     |
|   2  |        65%       |    18M   |     10    |        13       |       15     |
|   3  |        70%       |    20M   |     14    |        14       |       16     |
|   4  |        75%       |    22M   |     16    |        15       |       17     |
</UnitTable>


<SmallTitle>更新历史</SmallTitle>

<Timeline>
    <TimelineItem date="2024/11/25">
        <TimelineRow>17 本推出，并在 15 本新增复苏法术。</TimelineRow>
    </TimelineItem>
    <TimelineItem :historyBottom="true" />
</Timeline>