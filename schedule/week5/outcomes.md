<link rel="stylesheet" href="{{baseUrl}}/css/main.css">
<link rel="stylesheet" href="{{baseUrl}}/css/schedule.css">

<div class="website-content">

## Week 5 - Outcomes

<div id="main">

<!-- ==================================================================================================== -->

<include src="outcome-forkingWorkflow.md" />

<!-- ==================================================================================================== -->

<include src="outcome-junit.md" />

<!-- ==================================================================================================== -->

<include src="outcome-inheritance.md" />

<!-- ==================================================================================================== -->

<panel type="danger" header="**`W5.4` Can work with a 2KLoC code base** :star: ==[Compulsory]==" expandable>
  <panel header=":dart: Evidence" expanded>
<div id="lo-2kloc">

<tip-box type="important"> 
  This LO requires coordination and cooperation among team members. It also requires a few days to complete; we recommend that you start it early in the week rather than just before the tutorial day.
</tip-box>

#### Individual component:

**You can omit this individual component if** you have worked with a code base that meets the following criteria:
* more than 2KLoC of the code base was written by other developers
* your code included automated tests
* your code was contributed via a proper revision control workflow e.g. pull requests

**Requirements**: Do an enhancement to [[AddressBook - Level2](https://github.com/nus-cs2103-AY1718S1/addressbook-level2)]  %%e.g. add a new command%%. It can be the same enhancement you did to AddressBook Level1 (at the 1KLoC milestone in week 3). The size of the enhancement does not matter but you must,
* update the User Guide
* update existing tests and add new tests if necessary, for both JUnit tests and I/O tests
* follow the coding standard
* follow the OOP style

Optional but encouraged:
* Update the Developer Guide

Those who failed to produce working code at 1KLoC milestone (in week 3) can recover the lost marks by doing _two_ enhancements at this milestone.

#### Team component:

The team component is ==to be done by all members==, including those who were allowed to omit the individual component.

* Review PRs created by team members in the _Individual Component_ above. You can either give suggestions to improve, or ask questions to understand, the code written by the team member. Try to get each PR reviewed by at least one team member and try to ensure each team member's PR is reviewed by at least one other team member.  

<tip-box type="tip">
  
Note that you can reuse the code you write here in your final project, if applicable.
 
</tip-box>

<include src="submission.md" />

</div>
  </panel>
</panel>

<!-- ==================================================================================================== -->

<include src="outcome-classLevelMember.md" />

<!-- ==================================================================================================== -->

<include src="outcome-composition.md" />

<!-- ==================================================================================================== -->

<include src="outcome-aggregation.md" />

<!-- ==================================================================================================== -->

<include src="outcome-overloading.md" />

<!-- ==================================================================================================== -->

<include src="outcome-classDiagram.md" />

<!-- ==================================================================================================== -->
<!-- TODO:  
<include src="outcome-library.md" />
-->
<!-- ==================================================================================================== -->

<panel type="info" header="**`W5.10` Can explain single responsibility principle** :star::star::star:" no-close>
  <include src="../../book/principles/singleResponsibilityPrinciple/full.md" />
  <panel header=":dart: Evidence" expanded>

**Acceptable**: Evidence of having used SRP in some project.

**Suggested**: Do the exercise in [[Addressbook-Level2: LO-SRP](https://github.com/nus-cs2103-AY1718S1/addressbook-level2/blob/master/doc/LearningOutcomes.md#follow-the-single-responsibility-principle-lo-srp)]

<include src="submission.md" />

  </panel>
</panel>

</div>
</div>