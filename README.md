Download Link: https://assignmentchef.com/product/solved-cis301-homework-3-propositional-proofs
<br>
Purpose of Assignment:

To help you understand …

<ol>

 <li>natural deduction rules for propositional logic</li>

 <li>how to apply the rules for proving validity of sequents</li>

 <li>some properties of propositional logic connectives and how they can be proven using natural deduction</li>

 <li>how to determine provability</li>

</ol>

We have created some automated grading tools to speed the grading of homeworks. To apply those tools, we need to make sure that each student uses a consistent naming for all their solutions file. Therefore, we have created an IntelliJ project with template files for your solution. DON’T CHANGE THE NAME OF ANY OF THE FILES that we give you.

<h1 id="hints">Hints:</h1>

If you get stuck in a proof, take a look at the tactics given in the lecture slides associated with the operators involved in the formulae.

Typically, you’ll introduce from the inside-out and eliminate from the outside-in

<h1 id="gettingstarted">Getting started</h1>

You can find examples of completed Logika propositional proofs in the Logika example repository (included in the class examples that you downloaded (as illustrated in the “Step #2” videos). Here is a direct link to the propositional proofs portion of those examples:https://github.com/sireum/v3-logika-examples/tree/release/src/propositional

<h1 id="considerations">Considerations</h1>

<ol>

 <li>All files must run in the Sireum IVE</li>

 <li>“Proof” means “a Logika 2 column proof”. And “Prove” means “provide a proof”</li>

 <li>To receive any points a problem must:</li>

</ol>

<ul>

 <li>be a Logika Propositional Proof or Truth Table (see examples and class slides). Note: Each problem admits only one or the other</li>

 <li>contain the correct logical sequent</li>

</ul>

<ol>

 <li>Partial credit may be received if the proof is not finished.</li>

 <li>Correctly proven claims that do not progress the proof will not impact your grade</li>

 <li>Each provable sequent can be proven in at most 20 steps.</li>

 <li>Point values are proportional to difficulty.</li>

</ol>

<h1 id="problems">Problems</h1>

<ol>

 <li>(3 points) From homework 1, you may notice that for every case that <code>(p → q) → r</code> is true, <code>p → (q → r)</code> is true as well. To confirm this observation, prove <code>(p → q) → r ⊢ p → (q → r)</code> (Hint: https://github.com/sireum/v3-logika-examples/blob/release/src/propositional/implies/implies-4c.logika)</li>

 <li>(4 points) Prove <code>(p ∧ q ∧ r) ∨ s ⊢ (p ∨ s) ∧ (q ∨ s) ∧ (r ∨ s)</code> (Hint: consider proof to this sequents <code>(p ∧ q) ∨ r ⊢ (p ∨ r) ∧ (q ∨ r)</code>)</li>

 <li>(4 points) Prove <code>p ∨ (q ∨ r) ⊢ (p ∨ q) ∨ r</code></li>

 <li>(3 points) Prove <code>p → s ⊢ p ∧ q → r ∨ s</code></li>

 <li>(4 points) Prove <code>p → q ∨ r, q → s, r → t ⊢ p → (t ∨ s)</code></li>

 <li>The sequent <code>&lt;premise1&gt;, &lt;premise2&gt;, ... &lt;premiseN&gt; ⊢ &lt;consequent&gt;</code> is provable if and only if the formula <code>&lt;premise1&gt; ∧ &lt;premise2&gt; ∧ ... &lt;premiseN&gt; → &lt;consequent&gt;</code> is a tautology. This is equivalent to saying that a sequent is not provable if and only if there is some truth assignment for the variables where the formula evaulates to false. For each of the following sequents, either prove it or show that it is not possible with a truth table of the corresponding formula.Advice:</li>

</ol>

<ul>

 <li>You could practice Z3 by writing a program to determine if the sequent is provable. Feel free to submit a Z3 files but the autograder will ignore it.</li>

 <li>If you make a truth table that is a tautology, you’ve just shown the sequent is provable. You’ll need to make such a proof instead.</li>

 <li>If you make a truth table that is a contingent, notice the cases you enumerated when the formula is not true. These cases are counter examples to the claim that the sequent is provable. For these cases, the conclusion can not be derived from the premises.</li>

 <li>If you make a truth table that is a contradiction, you’ve shown that in no case can the conclusion be derived from the premises.</li>

 <li>Each completable proof takes at most 10 steps.a. (3 points) <code>p ∧ q ⊢ p → q</code>b. (3 points) <code>p → q ⊢ p ∧ q</code>c. (3 points) <code>p ∧ q → r ⊢ p → q → r</code>d. (3 points) <code>p → q → r ⊢ p ∧ q → r</code></li>

</ul>