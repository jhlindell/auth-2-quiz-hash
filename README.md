# Storing Passwords Quiz
## Would you like salt with your hash?


With your partner, in words both of you will understand 6 months from now, answer the following questions.

> A customer hires you to consult on a web app.  You notice that they are storing their passwords in plaintext.  What advice would you give the customer.  This advice should outline the risks of the current solution, and give a list of best practices for a new solution.

The advice I would give is that if they don't secure their passwords, they are leaving themselves open to a huge amount of liability. If plaintext passwords get stolen, the chance of lawsuits is good. I would recommend that their passwords policy be completely overhauled. Things to implement:
1. Generate a random salt to add to this password.
2. Use this salted password to generate a hash of the password.
3. Store the salt and passwords separately.
4. Profit.

> You are tasked for creating a RFP (request for proposal) for a new cryptographic hashing algorithm.  What requirements would you put in place for this new algorithm.

1. Algorithm be a one way algorithm.
2. The algorithm takes in plaintext and outputs scrambled text.
3. The algorithm always outputs the same length output.
4. No 2 text inputs will return the same output.
5. Small changes to the input text will result in huge changes to the output.
6. The algorithm should be slow, so that repeated attacks would be limited by the slow speed.
7. Algorithm is easy to implement.
