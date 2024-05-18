# NotDelayedAnymore 不在拖堂

一款基于`Python+Tkinter`的防拖堂软件，使用基于简单公式的随机密码进行解锁，有效防止大部分老师（仅针对无键盘环境）

开坑ing……

## 如何计算密码？

软件锁屏后会显示三个值`233≤Ka≤69696, 11451≤Kb≤19198, Kc=5`，其中Kc可视为剩余尝试次数。

密码可通过套用公式`P=[(Ka mod 233)+Kb-11451]*Kc`得来，其中`P`为最终密码数值。

## 紧急情况解锁不了怎么办？

右下角有红字按钮`紧急解锁`，每台设备有3次机会，点击弹出确认框，确认即可解锁。

或者在密码框中输入`EM_UNLOCK`解锁设备，效果一致。

当然也可等到下课时间自动解锁。
