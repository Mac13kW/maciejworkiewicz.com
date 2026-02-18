---
title: "Human-AI collaboration: The power of mental models"
date: 2023-12-15
lastmod: 2025-01-29
tags: ["AI", "problem solving", "GPT-4", "GPT-o1", "DeepSeek", "chess"]
description: "An experiment showing how LLMs fail at spatial reasoning with modified chessboards, highlighting the importance of mental models in strategic thinking."
---

A lot has been recently said about the tremendous impact that the current generation of large language models (LLMs) has and will have in the future on the functioning of organizations and competitive dynamics between them. A particularly intriguing prospect is the potential of these AI systems to eventually take on roles traditionally reserved for humans, like developing business strategies. While, at least to me, the answer to this question largely depends on the timeframe we assume until the full Artificial General Intelligence arrives, the intermediate period of collaboration between humans and AI also presents important questions regarding the nature of this collaboration and areas in which current LLMs still fall short.

Numerous studies have demonstrated remarkable productivity gains in managerial tasks when augmented by technologies like [GPT-4](https://openai.com/index/gpt-4/) or the new crop of "reasoning" AI models like [GPT-o1](https://openai.com/o1/) and [DeepSeek](https://www.deepseek.com/). These AI systems excel in processing vast datasets, solving problems in areas like mathematics, economics, and logical reasoning, or helping me copy-edit this article. However, when it comes to strategic decision-making—a subject I am deeply interested in and engage with both in research and teaching—there remain certain limitations to what current AIs can achieve. One of them is strategic foresight using mental models.

Strategic foresight requires a type and level of abstract thinking that current LLMs were not built to handle. This involves developing and using mental models that, while being simplified representations of reality, capture the critical elements of a real-world environment (see, for example, the excellent book by Newell and Simon [1972], who were awarded the Turing Award for creating the first AI programs). Interestingly, even very complex problems can be represented with only a few key parameters and be effective for guiding strategic decision-making (see Scott Page's 2018 "The Model Thinker" for example). These models enable decision-makers to envision future scenarios and respond proactively to evolving market dynamics where data is not yet available.

Take the Nokia case in 2007, for instance. Despite being a leader in mobile phone manufacturing, Nokia failed to anticipate the industry's shift towards smartphones, a change signaled by the launch of the iPhone in January that year. In 2007, Nokia was the absolute market leader when it came to mobile phone manufacturing and smartphone manufacturing. Magazines like Forbes have been openly doubting whether any company can ever catch up with the Finnish mobile manufacturer. However, the company didn't consider that change to the competitive landscape that the iPhone heralded. As mobile phones became more and more capable, they effectively became computers. Thus, the competitive advantage that was the source of success for mobile phone manufacturers, like manufacturing prowess, supply chain management, and relationships with mobile service providers, became less important, and capabilities characteristic of the computer industry, like software development and managing relationships with software developers to build platforms, became key. Working through the implications of such a change could have alerted the management to the shift in the competitive landscape. I am not claiming here that this is the only explanation for the company's subsequent fall from grace, but there's an important lesson about understanding or having the right representation of the environment – a representation that can be subsequently manipulated in one's head to help think through the implications of changes in that environment.

To illustrate how LLMs fail at this, I conducted a little experiment with GPT-4 in December 2023 and repeated it with GPT-o1 and the new DeepSeek R1 in January 2025, the latest iterations and arguably the most powerful of the new crop of LLMs. In this experiment, I asked the AI to consider a game of chess. First, I asked which player, White or Black, would be more likely to win a game of chess. GPT-4 correctly reported that while the chances of winning depended mostly on the skill of the players, if the players were evenly matched, the White player would have a slight advantage over the Black player, just because the White player moves first, and therefore has one more move and can also dictate the style and tempo of the game. The empirical record supports this. So far, so good.

Then I asked GPT-4 to consider two types of changes to the chessboard. In the first scenario, I asked AI to consider a cylindrical chessboard where the top and the bottom edge connect so that by stepping beyond the top edge, a piece would appear at the bottom and vice versa. In the second manipulation, I asked GPT-4 to consider a toroidal chessboard. A torus is an object where the top and the bottom edges meet and so do the left with the right edge, thus creating a continuous space. The resulting object has the shape of a doughnut with a hole in the middle.

#### Figure 1. A traditional chessboard

![image](/images/18_chess_wiki.jpg)

If you have ever played the Snake game on the standard Nokia phone, you recognize this type of space, where the snake loops over the edges. Then I asked GPT-4 to consider which player -- assuming other rules remain the same as in the classical game -- would win such a game on average.

Now, here I want you to stop for a moment and consider such a change. Imagine such a chessboard. You can start with the cylindrical one. Consider your first move as a White player. You can move forward as in the normal game of chess, but pieces can also move backward. Taking a step back would make you pop up at the top. Think about the moves that you can execute in such a situation. Take a minute. It will be worth it. Got it? OK, what do we get?

If you have played chess before or if you think through this example carefully, you will quickly realize that a White player always wins on such a chessboard. This is because the White player can simply move the king one step back, thus capturing the opponent's king in the first move! Once you consider this, it becomes obvious.

However, not for GPT-4, which doesn't have a mental model of the playing board in its digital brain. It simply assembles sentences using its algorithms based on the training set of texts (I know this is a gross oversimplification of how a generative pre-trained transformer works, but you get my point).

Interestingly, another generative AI, Midjourney, also doesn't have a representation of even the classical board of chess. I could not make it create an image of a chessboard with pieces in initial positions. Neither can DALL·E 3 via GPT-4.

#### Figure 2. Midjourney's attempts at classical chessboard

![image](/images/18_chess_2.png)

Note: the instruction was: "Show me a photorealistic classical chessboard with all the pieces set up to start the game of chess. All pieces are in their initial positions."

#### Figure 3. DALL·E 3 attempt at the classical chessboard
![image](/images/18_dalle_chess.png)

When I asked GPT-4 what would happen after the board has been changed in one of these two ways, it replied that it would most likely profoundly change the strategies available to the two players, but one cannot predict which player would win; however, the white player can still maintain a slight advantage in such a situation. I did this several times for both the cylindrical and the toroidal board and received essentially the same response.

This experiment is not intended to diminish the remarkable capabilities of LLMs but to highlight the crucial role of human insight in strategic decision-making. As we embrace these technologies, managers, students, and aspiring leaders need to cultivate the ability to think abstractly and develop a comprehensive understanding of competitive dynamics. This skill remains invaluable in a world where AI aids but does not replace the strategic acumen of human decision-makers. As we continue to leverage AI technologies, we must also commit to refining our strategic thinking skills with particular emphasis on building a robust set of mental models to help us understand and foresee changes in the environment. In this way, both players, humans and AI, win. For now.

#### Figure 4 - Examples of the GPT-4 experiment
![image](/images/18_GPT_chess.png)


I repeated the same exercise with GPT-o1 - the reasoning model. I asked it exactly the same questions. It got it wrong as well. Like before, it argued that the White player has a slight advantage due to simply moving first. Here is the concise answer I got from it:

*Even with the board’s top and bottom wrapped, White still retains a slight advantage by moving first, although the altered geometry changes the nature (but not the existence) of that advantage.*

The same happened with DeepSeek. It even claimed that:

*While White still holds a slight edge due to the first move, the advantage is smaller than in traditional chess. The cylindrical board’s increased tactical complexity and defensive options for Black (e.g., king mobility, counter-wrapping attacks) narrow the gap. However, White’s ability to initiate early threats in a high-mobility environment likely preserves a marginal win-rate advantage—closer to 50-50, but with White slightly favored (e.g., 51-49%).*

<!-- TODO: Add Figure 5 - Examples of the GPT-o1 experiment -->

#### Figure 5 - Examples of the DeepSeek experiment
![image](/images/18_DeepSeek_chess.png)

This is a space to watch. However, this type of reasoning, which is important from the point of view of strategic thinking and problem-solving, seems elusive for these models. For now.
