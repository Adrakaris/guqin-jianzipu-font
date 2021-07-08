# Guqin Jianzipu Notation

#### 古琴减字谱字体

This is a font for writing Jianzipu for the Guqin, based off Noto Sans SC.

We use ligatures to be able to type Jianzipu notation - these will be referred to as commands.

Only the ones included are shown.

## Overview of Use

First use a \ command to write a body block, then combine any number of / commands for the modifier blocks. **Do not write spaces.** Once the *full thing* has been written, *then* put a (halfwidth) space.

`\7g/da/76` will generate a block meaning 大指按7徽6分，勾7弦.

For any | (combining) blocks, **do not put a space** between that, the first block, and the second block.

`\4/da/10||\7/s` will generate a 撮 block with 4弦大指10徽 and 散音7弦.

## Notation

### \\ (Backslash)

Backslash commands refers to "body" blocks. Typing \\1 will render 一, up to \\7 for 七. These numbers can then be suffixed with letters, which refer to the right hand technique for that block. The examples shown use the 1st string, though this can be replaced with any number up to 7.

* **\\1g**: g stands for 勾 (**g**ou)
* **\\1t**: t stands for 挑 (**t**iao)
* **\\1m**: m stands for 抹 (**m**o)
* **\\1u**: u stands for 托 (t**u**o)
* **\\1d**: d stands for 打 (**d**a)
* **\\1b**: b stands for 擘 (**b**o)
* **\\1i**: i stands for 剔 (t**i**)
* **\\1mt**: mt stands for 抹挑 (**m**o **t**iao)
* **\\1mg**: mg stands for 抹勾 (**m**o **g**ou)
* **\\1gi**: gi stands for 勾剔 (**g**ou t**i**)

Other \\ commands are:

* **\\fan** (起) and **\\fanz** (止): indicates the beginning and end of 泛音 respectively
* **\\tao**: represents 搯
* **\\dai**: represents 带起
* **\\jin**: represents 进
* **\\tui**: represents 退
* **\\fu**: represents 复
* **\\zhu**: represents 撞
* **\\yin**: represents 吟
* **\\nao**: representts 猱
* **\\tan**: represents 淌
* **\\tuo**: represents 拖
* **\\dou**: represents 逗

### - (Dash)

Dash commands are used to represent slides. These are always typed the following way:

First, type either **-s** for 上 or **-x** for 下. 

*If you need a whole number hui* type a dash (**-**) followed by that number. You are done.

*If you need a fractional hui* first for the whole type **-z** (中) followed by that number. Then for the fraction type a dash (**-**) followed by that fraction.

`-s-7` means 上七徽. `-x-z10-8` means 下十徽八分.

*Note:* **-b** represents 半, **-w** represents 外, and both only appear in the bottom position. However, -5 is also valid for 半 and will display the character for 5 instead. 外 should not be used with any other modifier.

The middle numbers range from 1 to 13, the bottom numbers range from 1 to 9.

### / (Forwardslash)

Forwardslash commands refer to "modifier" blocks. These are the particles that go on top of the body such as 艹, and hui markers. *Finger indicators* and *Hui indicators* can be combined in any order. 

Basic / commands are:

* **/s**: represents 散音
* **/fa**: the single 泛音 indicator
* **/wai**: represents 外, a hui position outside of the main 13
* **/jiu**: represents 就
* **/ch**: represents 绰 - *note:* this is displayed above rather than below the hui position - this is to ensure ligature compatibility
* **/zhu**: represents 注 - *note:* will overlap with previous block if no spaces are between blocks


Finger / commands are:

* **/mi**: ring finger, 无名指
* **/zh**: middle finger, 中指
* **/sh**: index finger, 食指
* **/da**: thumb, 大拇指

Hui commands are written by writing the hui number, and then the fraction immediately after. 76 for example is 7徽6分, and 123 is 12徽3分. **Only standard hui positions are included** - to not make my life hell only the following combinations are included:

* All whole numbers from **4** to **13**
* **56** (5.6)
* **64** (6.4)
* **73** (7.3)
* **76** (7.6)
* **79** (7.9)
* **85** (8.5 or 8半)
* **108** (10.8)
* **123** (12.3)
* **131** (13.1)

### | (pipe)

Pipe commands are "combinator" commands. They are used for writing notation which combines two blocks, like 撮 notation. They go in the middle of two blocks to "combine" them. Both "arms" of the combinator encompass two fullwide spaces. 

* **||**: represents 撮, for optimal spacing do not put a space between the two encompassed blocks
* **|f**: represents 反撮.


## Attributions

Noto Sans SC is the base font, and is licensed under the [SIL Open Font License](https://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=OFL) and this is also licensed accordingly. The base font is also in this repository (for convenience). 

>  You can use them freely in your products & projects - print or digital, commercial or otherwise. However, you can't sell the fonts on their own.

> This isn't legal advice, please consider consulting a lawyer and see the full license for all details. 
