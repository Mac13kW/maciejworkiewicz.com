---
title: "Coding"

---

Even basic knowledge of computer programming can be very valuable for a social scientist. There are two key functionalities that are especially useful - automation and the random number generator. The first one is pretty straightforward; it increases researcher's productivity by having the computer perform tasks that would otherwise have to be completed manually. Modern programming languages like [Python](https://www.python.org/) or [R](https://www.r-project.org/) offer many powerful tools like data collection using web crawlers and text extraction from PDFs to data management and analysis, machine learning, and data visualization. Furthermore, with the development of modern powerful Large Language Models, like GPT-4, coding has never been easier and it will only get better.

The second functionality - the random number generator - opens doors to computational modeling and [Monte Carlo](https://en.wikipedia.org/wiki/Monte_Carlo_method) analysis, among others. While not as popular as empirical research methods, computational modeling is a powerful tool in helping us to better understand complex phenomena.

Links to my projects on [GitHub](https://github.com/Mac13kW).

---

### [A Basic NK Model](https://github.com/Mac13kW/NK_model)

This program creates an NK Model ([Kauffman, 1993](https://www.amazon.com/Origins-Order-Self-Organization-Selection-Evolution/dp/0195079515?ie=UTF8); [Levinthal, 1997](https://pubsonline.informs.org/doi/abs/10.1287/mnsc.43.7.934)) representing a task environment of varying degree of complexity (K) i.e. number of interdependencies between individual binary variables.

It produces multiple types of NK landscapes and saves them as numpy binary files, which contain all combinations, contributions of each combination of decision variables and information about whether a given combination of variables is a local peak (finds all combinations, from which single-variable deviations produce only worse fit).

---

### [The Garbage Can Model](https://github.com/Mac13kW/Garbage_Can_Model)

This is a recreation of the [Cohen, March and Olsen (1972)](https://www.jstor.org/stable/2392088?seq=1#page_scan_tab_contents) Garbage Can Model of organizational decision making in Python.

For those interested in how the model works I would point you to the original article first. You can then use the Python code to recreate the original results and play with the assumptions. Wherever possible I tried to preserve the original names of variables, vectors and matrices.

Some interesting points came out when recreating the code. One peculiar feature of the original model, for example, is that it allows decisions to be made when there are no decision makers attached to the problem. I added comments to the code to help you follow what I did.

---

### [A Simple Web Scraping Tool](https://github.com/Mac13kW/AOM_web_scraping)

In 2015 I taught a course to INSEAD PhD students and faculty on using Python for research as part of an initiative supported by Phanish Puranam. Together with Julien Clement (another INSEAD PhD student) we came up with an idea to create a two-day workshop where participants would learn how to create a script to crawl a set of websites and extract the information, which would be subsequently analyzed. I was responsible for the first part of the course - creating the web scraping Python program.

You can find the original code and the course slides with exercises on my GitHub website. It is a simple script but it should be a good starting point for those who want to learn the basics of web scraping. 

---

### [Robert Axelrod's PD Tournament](https://github.com/Mac13kW/PD_tournament)

This is a recreation of Robert Axelrod's tournament which pit many strategies against each other to find out which performed the best in a repeated Prisoner's Dilemma game.

I prepared this code for a PhD class at ESSEC. It helps students to understand the tournament and gain intuition for the game and why tit-for-tat performs so well.

I highly recommend reading the Robert Axelrod's excellent book "The Evolution of Cooperation". It is an excellent piece. Such a simple idea and yet it explains so much about the world - particularly the social sphere. If you were looking for mathematical foundations of morality, you will find them in this book.

The Prisoner's Dilemma has been a widely studied phenomena and the idea itself and numerous extension won Nobel Prize in economics for John Nash, John Harsanyi, and Reinhard Selten. The idea is very powerful and can help explain many market failures, including the problem with solving the climate change problem.

---

### [Central Limit Theorem](https://github.com/Mac13kW/Central_Limit_Theorem)

If you ever wondered how the CLT really works, but didn't find the mathematical proof enough? You can try this Python script to play around and explore how the distribution of the sample of means behaves in response to changing the number and size of each sample for a variety of distributions.

---

### [Comparing Distributions](https://github.com/Mac13kW/Comparing_distributions)

Experimental results often report statistically significant differences that are not very meaningful in everyday life, i.e. their actual impact is negligible. With big enough samples we can often detect differences, which magnitude is in fact very small.

This simple tool compares two normal, Poisson or Gamma distributions. Given the means and standard deviations of the distributions it will calculate a likelihood that a random draw from a population with a higher mean is bigger than a random draw from a population with the smaller mean. Such a comparison gives a good intuition regarding the size of the detected difference.

---

### [March 1991 Exploration and Exploitation without the access to the original code](https://github.com/Mac13kW/March_1991_Exploration_and_Exploitation)

This is a recreation of the computational model from [March JG. 1991. Exploration and Exploitation in Organizational Learning, Organization Science. 2(1):71-87](https://pubsonline.informs.org/doi/abs/10.1287/orsc.2.1.71?journalCode=orsc)

I recreated the model without access to the original code. The purpose of this exercise was to assess the ease of reproducing the original figures from the paper. In the process I made some interesting observations. For example, despite being somewhat easy to write the simulation as presented in the manuscript, it is difficult to reproduce the original figures. You can find my code (written in R) on my GitHub page. The code recreating the original figures will be coming shortly.

---

### [March 1991 Exploration and Exploitation - The Original Code](https://github.com/Mac13kW/March_1991_Original)

This is a second recreation of the computational model from [March JG. 1991. Exploration and Exploitation in Organizational Learning, Organization Science. 2(1):71-87](https://pubsonline.informs.org/doi/abs/10.1287/orsc.2.1.71?journalCode=orsc)

The code is based on the description from the paper itself (the relevant quotes are included in the code with a reference to page on which they appear in the original manuscript), but also on an article by Simon Rodan (2005) and especially the note by Michael Christensen (2015), both of which describe the missing steps necessary to recreate Figure 1 from the original paper. Attempting recreation of the model from the 1991 paper alone is not possible as the original text is missing important information. I provided specific notes in those places where the original code differs from the paper. I also wanted to thank Dong Nghi Pham, a doctoral student at ESSEC, who helped with reviewing the code.

---

### [Secret Santa](https://github.com/Mac13kW/Secret_Santa)

Produces matches between friends for a Secret Santa party. The script takes a list of names, creates a permutation with no fixed point and prints out each match.
