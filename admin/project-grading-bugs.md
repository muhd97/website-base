<div id="featureFlaws">

These will be considered _feature flaws_:<br>
:fas-bug: The feature does not solve the stated problem of the intended user i.e., the feature is 'incomplete'<br>
:fas-bug: Hard-to-test features<br>
:fas-bug: Features that don't fit well with the product<br>
:fas-bug: Features that are not optimized enough for fast-typists or target users
</div>

<div id="functionalityBugs">

These are considered _functionality bugs_:<br>
:fas-bug: Behavior differs from the User Guide<br>
:fas-bug: A legitimate user behavior is not handled %%e.g. incorrect commands, extra parameters%%<br>
:fas-bug: Behavior is not specified and differs from normal expectations %%e.g. error message does not match the error%%<br>
</div>

<div id="ugBugs">

These are considered UG bugs (if they hinder the reader):<br>
:fas-bug: Not enough visuals e.g., screenshots/diagrams<br>
:fas-bug: The visuals are not well integrated to the explanation.<br>
:fas-bug: The visuals are unnecessarily repetitive e.g., same visual repeated with minor changes.<br>
:fas-bug: Not enough examples e.g., sample inputs/outputs.<br>
:fas-bug: The explanation is too brief or unnecessarily long.<br>
:fas-bug: The information is hard to understand for the target audience. e.g., using terms the reader might not know<br>
:fas-bug: The document looks messy, or not well-formatted.<br>
</div>

<div id="dgBugs">

These are considered DG bugs (if they hinder the reader):

<panel type="seamless" header="Those given as possible UG bugs ...">
<include src="project-grading-bugs.md#ugBugs" />
</panel>

:fas-bug: UML notation incorrect or not compliant with the notation covered in the module.<br>
:fas-bug: Some other type of diagram used when a UML diagram would have worked just as well.<br>
:fas-bug: The diagram used is not suitable for the purpose it is used.<br>
:fas-bug: The diagram is too complicated.<br>
:fas-bug: Excessive use of code e.g., a large chunk of code is cited when a smaller extract of would have sufficed.<br>
</div>

<div id="bugCalculationNotes">

##### Notes on how marks are calculated based on PE product testing

* ==Of 3A and 3B above, the one you do better will be given a 70% weight and the other a 30% weight== so that your total score is driven by your strengths rather than weaknesses.
* Bugs rejected by the dev team, if the rejection is approved by the teaching team, will not be affect marks of the tester or the developer.
* The penalty/credit for a bug varies based on,
  * The severity of the bug: `severity.High` > `severity.Medium` > `severity.Low` > `severity.VeryLow`
  * The type of the bug:  `type.FunctionalityBug` > `type.DocumentationBug` > `type.FeatureFlaw`
* The penalty for a bug is divided equally among assignees.
* The developers are not penalized for the duplicate bug reports they received but the testers earn credit for the duplicate bug reports they submitted as long as the duplicates are not submitted by the same tester.
* <tooltip content="i.e., the same bug reported by many testers">_Obvious_ bugs</tooltip> earn less credit for the tester and slightly more penalty for the developer.
* If the team you tested has a low bug count i.e., total bugs found by all testers is low, we will fall back on other means %%(e.g., performance in PE dry run)%% to calculate your marks for system/acceptance testing.
* Your marks for developer testing depends on the _bug density_ rather than total bug count. Here's an example:
  * `n` bugs found in your feature; it is a difficult feature consisting of lot of code → 4/5 marks
  * `n` bugs found in your feature; it is a small feature with a small amount of code → 1/5 marks
* You don't need to find all bugs in the product to get full marks. For example, finding half of the bugs of that product or 4 bugs, whichever the lower, could earn you full marks.
* Excessive incorrect downgrading/rejecting/<tooltip content="marking as duplicates">duplicate-flagging</tooltip>, if deemed an unethical attempt to _game the system_, may be penalized.
</div>