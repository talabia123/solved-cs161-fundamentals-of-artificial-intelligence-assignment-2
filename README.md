Download Link: https://assignmentchef.com/product/solved-cs161-fundamentals-of-artificial-intelligence-assignment-2
<br>
<h1>Questions</h1>

<ol>

 <li>A search tree can be represented in LISP as follows:</li>

</ol>

<ul>

 <li>if the search tree contains a single leaf node <em>L</em>, it can be represented by atom L</li>

 <li>if the search tree has more than one node and is rooted at <em>N</em>, then it can be represented by a list (S1 S2 … Sk) where Si represents the <em>i</em>th subtree of <em>N</em>.</li>

</ul>

Consider for example the following search trees, whose LISP representations are shown later.

o              o                                      o                          o                   o

C     T  E     A

A                                H      R                EB

C

D

E

Write a single LISP function, called BFS. It takes a single argument FRINGE that represents a list of search trees, and returns a top-level list of leaf nodes, in the order they are visited by left-to-right breadth-first search. The inital call to BFS passes a FRINGE list with a single element: the root of the search tree.

Test your program on at least these inputs:

&gt; (BFS ’(ROOT))

(ROOT)

&gt; (BFS ’((((L E) F) T)))

(T F L E)

&gt; (BFS ’((R (I (G (H T))))))

(R I G H T)

&gt; (BFS ’(((A (B)) C (D))))

(C A D B)

&gt; (BFS ’((T (H R E) E)))

(T E H R E)

&gt; (BFS ’((A ((C ((E) D)) B))))

(A B C D E)

<ol start="2">

 <li>This question aims to solve a problem stated by Homer Simpson in <em>“Gone Maggie Gone”</em>, The Simpsons, Season 20, Episode 13. Watch the clip at <a href="http://www.simpsonsworld.com/video/313361987548">http://www.simpsonsworld.com/video/313361987548</a><a href="http://www.simpsonsworld.com/video/313361987548">. </a>Homer wants to cross a river with his baby (Maggie), his dog (Santa’s Little Helper), and a jar of poison. Homer is the only one who can operate the boat, and he can take at most one thing with him. The dog cannot be left alone with the baby, because he tries to bite her. The baby cannot be left alone with the poison, because she tries to eat it. The goal is to get everybody on the other side of the river.</li>

</ol>

The file <strong>hw2-skeleton.lsp </strong>contains a framework for solving this puzzle using depth-first search. Implement the functions in it as described in the comments. <strong>DO NOT CHANGE THE FUNCTION</strong>

<strong>NAMES OR PARAMETERS. DO NOT WRITE ANY ADDITIONAL FUNCTIONS</strong>.

<u>Extra: </u>watch the clip at <a href="http://www.simpsonsworld.com/video/313359939855">http://www.simpsonsworld.com/video/313359939855</a><a href="http://www.simpsonsworld.com/video/313359939855">.</a> It illustrates what happens when the search problem formulation ignores important details of the ill-defined real-world problem, and how the problem formulation is only an abstraction.


