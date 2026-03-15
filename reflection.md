# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
  The game looked ok but it was really buggy when I played it
- List at least two concrete bugs you noticed at the start  
  (for example: "the secret number kept changing" or "the hints were backwards").
  The hint only ever said go lower or go higher and that part was incorrect. The number that we were supposed to guess was -35 and that wasn't a possible option. Another time, I played it I saw that the hint kept saying go lower when it should have been saying go higher. Another thing I noticed is that the hard range is 1 - 50 while normal is 1 - 100. 

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
  I used Claude on this project.
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  One AI suggestion that was accurate was when it figured out the error with medium and hard levels was wrong and suggested a fix but before it did that it asked for verfication on what the hard level range should have been. 
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
  When I asked AI to implement two of the test cases that were required after fixing one of the errors, it never explicitely told me that pytest wouldn't be ready to run because there were still some unimplemented functions. So at first when I ran it, I was confused but then I realized I should have check the whole file instead of blindly running it. 

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
  I tested the game manually and made sure to focus on that specific bug while trying out multiple different possibilities.
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
  I ran a test case using pytest that AI generated to see if the 'GO HIGHER' and 'GO LOWER' were working correctly. According to pytest it did, so I knew my code was working after the fix.
- Did AI help you design or understand any tests? How?
  AI helped me design two tests. Once I asked it to implement a fix in my code, and based on that I said to create a test case that would check if you fix works.

---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
  The secret number is generated with a random number generater so each value in each game will be randomly generated.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
  Streamlit reruns are when someone interacts with the game and the program that works to run the game starts from the beginning.
- What change did you make that finally gave the game a stable secret number?
  Once the hints for guessing the value became more stable it became much easier to guess the secret number.

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
  Whenever I ask AI to make changes the to code, I always ask it to ask me first with what changes it's doing and what lines are specifically getting changed.
- What is one thing you would do differently next time you work with AI on a coding task?
  Especially when having AI fix errors, sometimes if it doesn't know the full scope of the problem it can often suggest wrong fixes. So double checking that information is something I would do differently the next time I work with AI.
- In one or two sentences, describe how this project changed the way you think about AI generated code.
  I used to think AI genetated code took longer than learning and coding assignments, but if used and prompted correctly, it can actually be a more efficient way to debug and work through any error while learning. 
