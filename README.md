# A) How to run:
1. Open terminal
2. Navigate to week3_automata
3. Run:
```bash
python3 demo.py
```
4. The last line of your output should read:
```bash
ALL TESTS MATCHED
```

# B) Challenges
The most difficult part about this project was implementing the NFA simulation correctly, particularly the management of the active state set at each step of execution.
Unlike a DFA, which maintains exactly one current state, an NFA may occupy multiple states simultaneously, requiring careful tracking of all possible computation paths.
Mistakes were easy to introduce when updating the active states after consuming each input symbol. Resolving these issues required closely examining the intermediate state sets produced during execution.

# C) Insight
The trace for 'abb' shows that NFA can track multiple paths at once but only accepts after the entire input reaches an accepting state. 
