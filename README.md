# Test2 PLC

**PLC Test2**

A) Rules for Recognizing all lexemes as their proper tokens

Tokens are a group of characters formingbasic, atomic chunk of syntax a "word"

Lexeme: group of characters that form a token
Token: class of lexemes that match a pattern

In this language, the type of tokens can be divided into few classes: keywords, identifiers, operators and punctuation, and delimiters.

![Image (1)](https://user-images.githubusercontent.com/79378418/202880181-60ddfaf0-dcc2-475d-b20e-c3ba0fc30cff.jpeg)
![2](https://user-images.githubusercontent.com/79378418/202880185-6dc50f98-3ccd-408b-a151-e31178a96928.jpeg)

![Image (2)](https://user-images.githubusercontent.com/79378418/202880173-77e063fc-9326-420f-8b6a-0521883e6e52.jpeg)
![Image (3)](https://user-images.githubusercontent.com/79378418/202880182-30979cea-3fda-481a-aca5-760e8fe2ad69.jpeg)

B) **EBNF Rules for my language**:
![Untitled 2](https://user-images.githubusercontent.com/79378418/202880292-886454b7-8bb1-45b8-9cc7-20289d842fdf.jpg)

C) **LL Grammar Test**

In order to conform with the norms of LL Grammar, it should pass the pairwise disjoint test and no LHR.

The grammar for my language is pairwise disjoint. It checks for every possible terminal symbol for each rule a
nonterminal has and makes sure they are all unique.Also, every first token in our grammar is unique which passes the pairwise disjoint test.

My grammar does not have any rules that cause left hand recursion, in which a nonterminal calls itself as the first character. No state here is calling itself, which proves there is no left hand recursion. In our grammar, there does not exist a non terminal that has multiple rules for one terminal. 

D) **Ambiguity Check** 

Generally, ambiguous grammar has multiple places where they are generating the same non-terminal in different positions. Our grammar does not have any such non terminals which are in different positions. My grammar also passes the LR Parser Test. A grammar is LR(1) if the following two conditions are satisfied for each configurating set: 1. For any item in the set [A –> u•xv, a] with x a terminal, there is no item in the set of the form [B –> v•, x]. In the action table, this translates no shiftreduce conflict for any state. Also, there is no right hand or left hand recursion in this grammar.

E) **Code in files** 

F) **Code in files**. 

G) **Test Files in repository**. 

H) **LR Parse Table**:
!![Untitled 4](https://user-images.githubusercontent.com/79378418/202880551-e21cd001-1605-4c57-b5fc-c071e2b2e4ec.jpg)
![Untitled 5](https://user-images.githubusercontent.com/79378418/202880562-55688789-f2b4-4cc8-8283-3b87a4f1194e.jpg)

![LR3](https://user-images.githubusercontent.com/79378418/202880534-bf40a4c6-698a-4399-bcad-acfd03703587.jpg)
