---
title: "On the pleasures of wasting time or on recreating March 1991 original code"
date: 2019-10-04
tags: ["computational modeling", "March 1991", "Python", "exploration exploitation"]
description: "Recreating the famous March 1991 Exploration and Exploitation model in Python."
---

In the first year of my PhD course I recreated the March 1991 model in Excel. It wasn't required, but isn't academic career about doing what you want and being paid for it? Well, I digress. I wrote a lot of bad code at that time, but the model worked and produced some results that corresponded to March's figures. However, there were some small discrepancies, which back then I took for a product of the original model being run for only 80 iterations per condition.

Later, I found out that March 1991 model is notorious for being difficult to recreate due to some differences between the model's description in the paper (and the infamous Footnote 1) and the actual code that was used to produce the results. Luckily, Simon Rodan (2005) and Michael Christensen have managed to obtain the original code and recreate the original figures with much greater fidelity.

Now, several years later, I finally got around to recreate the original model in Python (version 3.7). Rodan's and Christensen's work has been very helpful in this endeavor as was help from one of the doctoral students at ESSEC, Dong Nghi Pham, who helped me to review the code. Below is Figure 1 recreated with 100,000 iterations per parameter combination. The code can be found on my [GitHub website](http://github.com/Mac13kW/March_1991_Original).

<!-- TODO: Add Figure 1 - March 1991 recreation -->
