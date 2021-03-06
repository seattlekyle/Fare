Fare - [F]inite [A]utomata and [R]egular [E]xpressions
===================

<p>Project Fare is an effort to bring a <a href="http://en.wikipedia.org/wiki/Deterministic_finite-state_machine" target="_blank" title="Deterministic finite-state machine">DFA</a>/<a href="http://en.wikipedia.org/wiki/Nondeterministic_finite-state_machine" target="_blank" title="Nondeterministic finite-state machine">NFA</a> (finite-state automata) implementation from Java to .NET.&#0160;There are quite a few implementations available in other languages today. This project aims to fill the gap in .NET.</p>
<p>Fare is a .NET port of the well established Java library <a href="http://www.brics.dk/automaton/" target="_blank" title="dk.brics.automaton">dk.brics.automaton</a> with API as close as possible to the corresponding dk.brics.automaton classes.</p>

Development environment
-----------------------

* Microsoft Visual Studio 2010
  * .NET Framework 3.5
* ReSharper 6.0 Build 6.0.2202.688
* StyleCop 4.6.3.0
* AutoFixture 2.4.1
  * xUnit.net data theories
* xUnit.net 1.8.0.1549

Design changes
--------------

* Included a .NET port of [Xeger] (http://code.google.com/p/xeger/), for generating random text from regular expressions. Xeger does <i>not</i> support all valid Java regular expressions. The full set of what is defined here and is summarized at (http://code.google.com/p/xeger/wiki/XegerLimitations).
* Implemented object equality.
* Many getters and setters have been replaced by .NET properties.
* Many foreach loops have been converted to LINQ-expressions.
* Notes from porting Java code in .NET can be found [here] (http://www.nikosbaxevanis.com/bonus-bits/2011/11/notes-from-porting-java-code-to-net.html).

<i>Based on version 1.11-8 of dk.brics.automaton released on September 7, 2011. [ChangeLog] (http://www.brics.dk/automaton/ChangeLog)</i>