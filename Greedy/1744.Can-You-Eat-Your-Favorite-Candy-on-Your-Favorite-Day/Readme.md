### 1744.Can-You-Eat-Your-Favorite-Candy-on-Your-Favorite-Day

本题就是简单的贪心法。我们令每个query对应的天数为d，糖的种类为t，每日吃糖的极限是cap。

如果我们慢到极限，每天只吃一颗糖，经过d-1天时就已经把前t种的糖都吃掉了，那么在第d天肯定就吃不到第t种糖。

反之，如果我们每天吃到极限cap，经过d天后时，仍然还没有吃到第t种糖（最多只吃完了前t-1种糖），那么也宣告失败。

其余情况下，我们都可以调节每天吃糖的数量在1\~cap之间，使得在第d天的时候有机会吃到第t种糖。
