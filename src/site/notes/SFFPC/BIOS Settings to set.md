---
{"dg-publish":true,"permalink":"/sffpc/bios-settings-to-set/","noteIcon":""}
---

> [!Tip]
> Enter **BIOS** by pressing **F7**
##### PCI-e Riser Settings:
- Should I set it to PCI-e 3? or 4? *I think that I should set it to PCI-e 3 speed*

##### Ram:
- Go to **Main** tab to check if your RAM is running at full speed instead of 4800 Mhz, or else, set it to the speed that you bought the ram, it is 5800 Mhz I suppose.

##### CPU undervolting:
- Go to the **Advanced** tab.
- At the bottom, there is **AMD Overclocking**, select that and **accept** the warning.
- Then go to **Precision Boost Overdrive** screen and set **Precision Boost Overdrive** to **Advanced**.
- Set **PBO Limits** to **Auto** or **Motherboard**.
	- ==Motherboard== let's you have higher temps/performance. So choose the one you find more useful in your case.
- Then go to the **Curve Optimizer** at the bottom of this screen. This is where the amount of undervolting is set. The **simplest** way is undervolting **all the cores** the **same** amount.
	- Set **Curve Optimizer** value to **All Cores**.
	- Set the **All core curve optimizer sign** value to ==negative== since we are **undervolting**.  
	- The **All Core Curve Optimizer Magnitude** is the number of milivolts to adjust the curve. With simple words, the value that you put here is undervolting value, and the bigger the value, the bigger the undervolt is.
		- Start off with 15. Then boot into Windows, run stress tests and benchmarks to test it.
		- If it succeds, set the value to 20. Then again boot into Windows, run stress tests and benchmarks to test it. 
		- If it succeeds, set the value to 25 and repeat the benchmark operations.
		- If it succeeds again, set the value to 30 and repeat the benchmark operations. The guy who wrote this guide is using it at 30, so you can start expecting instability after this value.
		- If it succeeds again, set the value to 35, till the bencharmak..etc fails. Once you start facing poblems, boot into BIOS and put the previous value that you had which was stable, this is kind of your limit.
- How about **PPT** and **Thermal limit** settings? 

> [!Tip] 
> Here is the [link](https://www.reddit.com/r/sffpc/comments/18f68b4/simple_precision_boost_overdrive_undervolting/) to the guide above.