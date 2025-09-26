# **Problem: Zombie Hunt Survival**

### **Story Context**

You are forced to play the deadly game **Zombie Hunt** inside the **National Institute of Virus Research**.
Each player starts with **7 cards**, which may include:

- **Normal cards** → ranks A–K across suits ♦ ♥ ♣ ♠, each with a numeric value.
- **Zombie cards (Z)** → infect humans.
- **Shotgun cards (S)** → kill zombies.
- **Vaccine cards (V)** → cure zombies.

Players face each other over multiple rounds. The outcome of each duel determines whether they survive as humans, become zombies, or are eliminated. At the end of the game, whichever side (Humans vs. Zombies) has the most surviving players wins.

---

### **Rules**

1. **Playing Cards (Matching Suit Rule):**

   - In each round, players must **play one card**.
   - If a player is assigned a suit (♥, ♦, ♣, ♠), they must play a card of that suit if they have one.
   - If they have no matching suit, they may play a **special card (Z, S, V)** instead.

2. **Normal vs Normal (both human):**

   - If both play normal cards of the assigned suits, the winner is decided by comparing the **cumulative total of all normal cards remaining in their hand (including the one just played)**.
   - The winner **takes one card** from the loser’s hand.

3. **Zombie Card (Z):**

   - Defeats any normal card.
   - The losing player becomes infected → converted into a Zombie and gains an extra `Z` card in their hand.

4. **Shotgun Card (S):**

   - Can be played against a Zombie.
   - Instantly eliminates the Zombie player.
   - Ineffective against humans.
   - Disappears after one use.

5. **Vaccine Card (V):**

   - Played against a Zombie card, it cancels the infection and cures the zombie back into a human.
   - Cannot be used on oneself.

6. **Game Over Conditions:**

   - A player is eliminated if they run out of **normal cards**.
   - A zombie player is eliminated if killed by a **Shotgun**.
   - At the end of all rounds, the side with fewer members (Humans or Zombies) is eliminated.

7. **Game Clear Condition:**

   - A player survives all rounds and belongs to the majority side (Humans or Zombies).
