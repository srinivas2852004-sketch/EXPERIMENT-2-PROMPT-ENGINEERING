date:19-08-25
reg no:212222080051
EXP-2-PROMPT-ENGINEERING-
Aim:
Comparative Analysis of different types of Prompting patterns and explain with Various Test Scenarios

Comparative Responses: ChatGPT vs Gemini
Scenario 1: Mathematical Problem (7^13 mod 11)
Prompt (Chain-of-Thought): “Solve step by step: compute 7^13 mod 11 using modular arithmetic rules.”

ChatGPT: “Let’s compute step by step: 7 mod 11 = 7 7² = 49 → 49 mod 11 = 5 7⁴ = (7²)² = 25 → 25 mod 11 = 3 7⁸ = (7⁴)² = 9 mod 11 Now 7¹³ = 7⁸ × 7⁴ × 7¹ = (9 × 3 × 7) mod 11 = 189 mod 11 = 2. Final Answer = 2.”

Gemini: “7^13 mod 11 = 2. Explanation: 7² ≡ 5 mod 11 7⁴ ≡ 3 mod 11 7⁸ ≡ 9 mod 11 Multiply: 9 × 3 × 7 ≡ 2 mod 11.”

Difference:

ChatGPT = Detailed tutor style (step-by-step for learners).

Gemini = Quick reference style (short proof for experienced users).

Scenario 2: Funny Birthday Wish
Prompt (Persona): “You are a stand-up comedian. Write a witty birthday wish for a friend turning 25.”

ChatGPT: “Happy 25th! You’re officially old enough to know better but still young enough to ignore that advice. Don’t worry — 25 is just level 2 of adulthood, and the boss fight is bills!”

Gemini: Happy 25th birthday! You know, 25 is a weird age. You're old enough to rent a car without a massive surcharge, but you're still young enough that you'll probably get lost trying to find the rental agency. Enjoy the quarter-life crisis—it's like a midlife crisis, but with worse credit and a lot more ramen.

Difference: ChatGPT = more story-like humor. Gemini = punchline-style joke, short and snappy.

Scenario 3: Customer Support
Prompt (Instruction + Context): “You are a helpful customer support assistant. The customer’s order is delayed. Respond politely, provide tracking steps, and suggest escalation if needed.”

ChatGPT: “I’m really sorry your order hasn’t arrived yet. Could you please provide your order ID so I can check the status? In the meantime, you can track your package through your account. If the package doesn’t arrive in the next 2 days, I’ll be happy to escalate this to our logistics team for a faster resolution.”

Gemini: We apologize for the delay with your order. We understand this is frustrating, and we're here to help.

The current estimated delivery date is delayed due to an unforeseen shipping issue.

Track Your Order You can get the most up-to-date information on your package by following these steps:

Check your email: Look for a shipping confirmation email from us.

Find the tracking number: The tracking number is a long string of letters and numbers.

Use the carrier's website: Copy and paste the tracking number directly into the search bar on the shipping carrier’s website (e.g., FedEx, UPS, or USPS).

Difference: ChatGPT = empathetic + structured. Gemini = direct and action-focused.

Scenario 4: Technical Explanation (TDMA Sectoring)
Prompt (Chain-of-Thought): “Step by step, explain how sectoring improves capacity in TDMA: define TDMA, explain cell reuse and interference, compare 60° vs 120° sectors.”

ChatGPT: “TDMA (Time Division Multiple Access) divides channels into time slots… Sectoring reduces co-channel interference by splitting cells into smaller angular regions.

120° sectoring → 3 sectors per cell, moderate interference reduction, simpler implementation.

60° sectoring → 6 sectors per cell, stronger interference reduction, higher capacity but more hardware cost. Conclusion: 60° sectoring offers the best interference management, though at higher complexity.”

Gemini: What is TDMA? Time Division Multiple Access (TDMA) is a channel access method that allows multiple users to share a single radio frequency channel by dividing the signal into unique time slots. In a TDMA system, each user transmits and receives data in a rapid, pre-assigned sequence, one after the other. This prevents multiple users from transmitting on the same frequency at the same time, thus avoiding collisions and allowing for more efficient use of the available radio spectrum. A common analogy is a group of people sharing one microphone by taking turns speaking for a short, specific amount of time.

Cell Reuse and Interference Cellular networks are designed with a concept called frequency reuse to maximize the use of a limited radio spectrum. The entire geographic service area is divided into cells (often represented as hexagons), and a unique set of radio channels is assigned to each cell. Cells that are far enough apart can reuse the same set of channels without causing significant interference.

However, if cells using the same frequency channels are too close, their signals can interfere with each other. This is known as co-channel interference. The quality of a call or data connection is determined by the Signal-to-Interference Ratio (SIR). A high SIR is necessary for a clear signal, and interference from other cells can degrade this ratio, leading to dropped calls and poor performance.

How Sectoring Improves Capacity Sectoring is a key strategy for mitigating co-channel interference and increasing network capacity. Instead of using a single omni-directional antenna at the base station (which broadcasts a signal in all directions), a cell is divided into smaller, wedge-shaped sectors, each served by a directional antenna.

Each sector is assigned a dedicated set of channels from the overall cell's channel pool. Because the directional antennas focus their signal on a specific area, they reduce the amount of energy that spills into neighboring co-channel cells. This reduction in interference allows cellular planners to place cells using the same frequencies much closer together, thus increasing the number of channels available per unit area.

Interference Reduction: The most significant benefit of sectoring is the reduction of co-channel interference. By focusing the signal in a specific direction, the directional antenna minimizes the number of interfering signals from co-channel cells, improving the SIR.

Increased Frequency Reuse: A higher SIR allows for a smaller frequency reuse factor (the number of cells in a cluster before a frequency can be reused), which directly translates to a higher system capacity. More users can be served within the same geographic area.

Comparison: 60° vs. 120° Sectors The choice between a 60° and a 120° sectoring scheme is a trade-off between interference reduction and system complexity.

120° Sectors (3-sector Cell) A cell is divided into three 120° sectors.

Interference Reduction: This configuration significantly reduces the number of first-tier co-channel interferers from six (in an omni-directional cell) to just two.

System Capacity: It allows for a smaller frequency reuse factor, leading to a substantial increase in capacity (often around a 2-fold increase compared to an omni-directional cell).

Complexity: The system requires three directional antennas per cell. It also results in a higher number of handoffs as a mobile user moves between sectors within the same cell.

Trunking Efficiency: Because the total channel pool is divided among three sectors, the number of channels per sector is smaller. This slightly decreases trunking efficiency (the ability to efficiently handle traffic), meaning a larger channel pool is needed to achieve the same blocking probability.

60° Sectors (6-sector Cell) A cell is divided into six 60° sectors.

Interference Reduction: This is the more aggressive approach. It reduces the number of first-tier co-channel interferers from six to just one in the most ideal cases. This provides a greater improvement in SIR than 120° sectoring.

System Capacity: It allows for an even smaller frequency reuse factor, offering the highest capacity gains.

Complexity: This setup is more complex and expensive due to the need for six directional antennas per cell.

Trunking Efficiency: Dividing the channels into even smaller groups per sector further reduces trunking efficiency, a major drawback. More frequent handoffs are also required due to the smaller sector size.

Difference: ChatGPT = in-depth, layered, comparative. Gemini = condensed summary.

Scenario 5: Teaching a Language (Beginner Japanese)
Task: Teach a beginner how to use the Japanese particle "を (wo / o)" in sentences.

Prompts & Responses Broad Prompt

“Explain how to use the Japanese particle を.”

ChatGPT: “を marks the direct object of a verb in Japanese. For example, in ‘パンを食べます’ (pan o tabemasu), ‘パン’ (bread) is the object, and ‘食べます’ (eat) is the verb. It shows what is being acted upon. Another example: ‘映画を見ます’ (eiga o mimasu) = ‘I watch a movie.’”

Gemini:

Marking the Direct Object This is the primary function of を. It indicates what receives the action of the verb.
Structure: Subject + を + Direct Object + Verb

Examples:

私は本を 読みます。(Watashi wa hon o yomimasu.)

I book (direct object) read.

"I read a book."

彼はりんごを 食べました。(Kare wa ringo o tabemashita.)

He apple (direct object) ate.

"He ate an apple."

彼女は音楽を 聞きます。(Kanojo wa ongaku o kikimasu.)

She music (direct object) listens to.

"She listens to music."

Key Points:

The verb must be a transitive verb (a verb that takes a direct object). Intransitive verbs (verbs that don't take a direct object, like "to sleep" or "to go") do not use を.

The particle を comes after the noun it modifies.

ChatGPT = richer explanation + extra examples. Gemini = concise, dictionary-style definition.

Overall Comparison
Pattern	ChatGPT Style	Gemini Style
Zero-Shot	Explains + sometimes adds context	Short factual answer
Few-Shot	Imitates examples in tone	Mimics examples but more concise
Chain-of-Thought	Step-by-step, very detailed	Minimal but correct reasoning
Persona	Fully adopts role (creative/humorous)	Lighter role-play, sticks to brevity
Instruction + Context	Empathetic, structured, professional	Direct, efficient, less emotional
Broad Prompt	May over-explain	Often returns short, factual response
Result
ChatGPT shines as a teacher, explainer, and creative assistant. It provides depth, empathy, and interactivity, making it ideal for education, customer support, and content creation.

Gemini shines as a fast, factual assistant. It provides concise, efficient answers, making it ideal for quick lookups, summaries, and straightforward tasks.

The best results come when the prompting pattern matches the task:

Chain-of-Thought for math/technical (ChatGPT stronger).

Persona/Few-Shot for writing & teaching (ChatGPT stronger).

Instruction + Context for support & summaries (both good, Gemini more concise).


