{% from "common/macros.njk" import embed_topic, thumb with context %}
{% from "common/admin.njk" import show_admin_page with context %}

{% call show_admin_page("participation") %}
<div id="main">

**To receive full {{ marks_participation}} marks allocated for participation, meet the criteria {{ thumb("A", "info") }}, {{ thumb("B", "info") }}, and {{ thumb("C", "info") }}.**

**{{ thumb("A", "info") }} Earned at least half of weekly participation points in at least 10 weeks.**
<div tags="m--cs2103">

  * In-lecture quiz:
    * Answered at least 80% of the questions correctly: 2 points
    * Answered 40-80% questions correctly: 1 point
  * Post-lecture quiz:
    * Answered at least 80% of the questions correctly: 3 points
    * Answered 60-80% questions correctly: 2 points
    * Answered 40-60% questions correctly: 1 point
  * Missing compulsory administrative requirements %%e.g., forgot to submit peer evaluations%%: -2 for each miss
</div>
<div tags="m--cs2113">

  * Programming exercise (if any):
    * Submitted correct solutions at least 75% of the exercises: 3 points
    * Submitted correct solutions to 50-74% of the exercises: 2 points
    * Submitted correct solutions to 25-49% of the exercises: 1 point
  * Post-lecture quiz (if any):
    * Answered at least 75% of the questions correctly: 3 points
    * Answered 50-74% questions correctly: 2 points
    * Answered less than 50% questions correctly but answered more than 50% of the questions: 1 point
  * Compulsory administrative tasks %%e.g., submitting peer evaluations%%: 2 for each task
</div>

<div class="indented">

<span tags="m--cs2103">

{{ icon_info }} As the lecture on Week `N` covers topics for Week `N+1`, the Lecture `N`'s in-lecture and post-lecture quiz points are counted for Week `N+1`
</span>
<span tags="m--cs2113">

{{ icon_info }} Lecture in week `N`:
* In-lecture quiz and other activities are counted for week `N` lecture participation.
* Post-lecture quiz (if any) is counted for Week `N+1`
</span>
</div>

**{{ thumb("B", "info") }} Received good peer evaluations**

<div class="indented">

{{ embed_topic("peerEvaluations-midterm.mbdf#teamMemberEvaluation-conduct", "Admin " + icon_embedding + " Peer Evaluations → Criteria (Conduct)", "3") }}
{{ embed_topic("peerEvaluations-midterm.mbdf#teamMemberEvaluation-competency", "Admin " + icon_embedding + " Peer Evaluations → Criteria (Competency)", "3") }}

* -1 for each _professional conduct_ criterion in which you score below average (based on the average of ratings received).
* No penalty for scoring low on _competency criteria_.

</div>

**{{ thumb("C", "info") }} Tutorial attendance/participation not too low**

<div class="indented">

Low attendance/participation can affect participation marks directly (i.e., attended fewer than 7) or indirectly (i.e., it might result in low peer evaluation ratings).
</div>

<panel type="info" header="**+ Bonus Marks**" expanded no-close no-switch >

In addition, you can receive bonus marks in the following ways. Bonus marks can be used to top up your participation marks ==but only if your marks from the above falls below {{ marks_participation }}==.
* [For lecture participation] Received at least half of the points for lecture activities in at least 10 lectures: 1 mark
  * In-lecture quizzes (using pollev.com): scoring is similar to the post-lecture quizzes
  * Other in-lecture activities: scoring is case-by-case basis
* [For perfect peer ratings] Received good ratings for all 10 peer evaluations criteria: 1 mark
* [For helping classmates] Was very helpful to classmates %%e.g., multiple helpful posts in forum%%: 1 mark

</panel>
<p/>


{{ thumb("Examples:", "secondary") }}

* Alicia earned 1/2, 3/5, ++2/5++, 5/5, 5/5, 5/5, 5/5, 5/5, 5/5, 5/5, 4/5, 5/5 in the first 12 weeks. As she received at least half of the points in 11 of the weeks, she gets 5 participation marks. Bonus marks are not applicable as she has full marks already.
* Benjamin managed to get at least half of the participation points in 9 weeks only, which gives him 5-1 = 4 participation marks. But he participated in 10 lectures, and hence get a bonus mark to make it 5/5.
* Chun Ming met the participation points bar in 8 weeks only, giving him 5-2 = 3 marks. He lost 2 more marks because he received multiple negative ratings for two criteria, giving him 1/5 participation marks.

<panel type="info" header="##### Where to find your participation marks progress" expanded no-close no-switch >

**Your participation progress can be tracked in [this page]({{ url_participation_dashboard }})** from week 3 onward.
</panel>

</div>

{% endcall %}
