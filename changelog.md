Removed
=======


ToDo Fragen

* Bernhard möchte "qualitative case study" in "qualitative evaluation" umbenennen. Bekommen wir dann nicht Probleme, weil wir mit dem Wort Evaluierung den Mund vielleicht etwas zu voll nehmen?
	* Antwort: Wir sollten bereits von begin an davon sprechen, dass wir Back Pain als Case für unser Programm verwenden. Am Ende: Weitere in Aussicht!
	* Qualitative Case Study streichen - nur von Case Study sprechen!
* Nach Variables suchen und schauen, ob man es durch Features ersetzen kann

Changelog
=========

ToDo Submission:
* Remove Packages
* remove the keyword "Visualization System and Toolkit Design"
* Cramers V Contingency Values are calles "Contingency Pane"

Summary
=======

At first, we'd like to thank all reviewer for the detailed feedback on this paper. It helped us to present a much better publication! The work underwent substantial changes and enhancements. We extended the data used, made a new qualitative evaluation, revised all figures and focus on a more precise distinction to related work.

This cover letter is divided into two parts. The first highlights major changes to the paper. The second part covers the reviewer feedback as inline comments to the individual reviews.

Changes
=======

The Data
--------

* We extended the analysis to more subjects. We now cover 6.753 subjects and 2.440 segmented lumbar spine shapes. This allows for more statistical resilient results.
* As the epidemiologists are very enthusiastic about the work, there are currently a few applications for new data sets. Unfortunately, these processes take very long and most likely have to happen in an iterative way. But it demonstrates well, that epidemiologists are really interested in such systems

Abstract
--------

* [Reviewer 2, Reviewer 3] The abstract was completely rewritten with focus on the reviewer comments.

Introduction
------------

* We revised most parts of the introduction in order to highlight contributions and distinction to other work.

Epidemiological Data
--------------------

* [Reviewer 1] Reviewer 1 requested more details about the data and the challenges thereof.
	* We enhanced Section '2.2 Epidemiological Data' with challenges associated with epidemiological data.
	* Section '6.1 The Lumbar Spine Data Set' now describes the data in more detail.

Related Work
------------

* We reworked the related Work section completely. It now reflects on the impact of each presented publication to our work.
* The section concludes by highlighting the uniqueness of our work, compared with the presented papers.
* We added the following publications as requested by the reviewers:
	* T.Lammarsch, W.Aigner, A.Bertone, S.Miksch, and A.Rind. Towards a concept how the structure of time can support the visual analytics process. In Proc. of the Int. Workshop Visual Analytics, pages 9–12, 2011.
	* P. Angelelli, S. Oeltze, C. Turkay, J. Haasz, E. Hodneland, A. Lundervold, B. Preim, and H. Hauser. Interactive visual analysis of heterogeneous cohort study data. IEEE Computer Graphics and Applications, 2014. in print.
	* M. Q. Wang Baldonado, A. Woodruff, and A. Kuchinsky. Guidelines for using multiple views in information visualization. In Proc. of the Working Conference on Advanced Visual Interfaces, pages 110–119. ACM, 2000.
	* C. Weaver. Cross-filtered views for multidimensional visual analysis. IEEE Transactions on Visualization and Computer Graphics, 16(2):192– 204, 2010.
	* J. W. Emerson, W. A. Green, B. Schloerke, J. Crowley, D. Cook, H. Hofmann, and H. Wickham. The generalized pairs plot. Journal of Computational and Graphical Statistics, 22(1):79–91, 2013.
* [Reviewer 1] We choose Baldonado's work on coordinated multiple views over the one of Roberts, since we found it fitted better for our paper.
* [Reviewer 2] We decided against including Intelligent visualization and exploration of time-oriented data of multiple patients of Klimov et al.. It's major focus in on analyzing time-oriented data and the efficient selection of subject groups sharing a certain condition and tracking it over time. It relies heavily on hypothesis based data analysis. Since we ran out of space, we did not include this work, because we cover publication based on the time factor and explained the difference of our approach on these works.

System Design and Implementation
--------------------------------

* Section `5 System Design and Implementation` now describes detailed each part of the system, how it was designed and also argues, why we made certain design decisions. These decisions are also supported by expert feedback.
* [Reviewer 2] Reviewer 2 noted that "In Figure 3 left there are 4 body size groups but on the right and in  the small image above the arrow there are only 3 groups." This is due to the the mapping on gender, the size-group 139-153.5 cm is only populated by women, while 182.5-197 contains only men.

Background
----------

* [Reviewer 2] Information about `Simpsons Paradox` added. Reviewer 2 pointed out a possible relation between confounders and Simpsons Paradox. The Reviewer is right, since Simpsons Paradox is a very extreme case of a confounder (http://www.bmj.com/content/309/6967/1480). We added information about this to the background chapter, but due to space problems we had to remove it again. This paper is to recommend :[19] S. A. Julious and M. A. Mullee. Confounding and simpson’s paradox. BMJ, 309(6967):1480–1481, 12 1994. Here is the text, which was cut:
		* An extreme form of confounding is called \emph{Simpson's Paradox} \cite{SimpsonsParadox}, where the confounder reverses the observed effect between two features. A famous example is the Berkeley University gender bias case, where significantly less women were admitted. Analysis later showed that women applied mostly for strongly restricted subjects and when only looking at acceptance divided by departments there was actually a small bias toward women.

Implementation
--------------

* Due to the lack of space we did not expand the `Implementation` section. Also Reviewer 2 and Reviewer 1 made contrary statements about whether the section should be extended or shortened.
* [Reviewer 3] The R shiny package does allow to use R code on the web, but in a very closed manner, you have to use their system (and ideally the RStudio IDE) to make this work. If you are interested in usages of R in a web context outside of Shiny, you can have a look at (RServe)[http://rforge.net/Rserve/]. I made an interface a year ago for RServe to Node.js, but its more a proof of concept thing (https://github.com/Powernap/rserve-js-Interface). For this work it was way easier though to implement the statistics algorithms from scratch, eliminating the need to work with another local server, like RServe.
    * These possibilities are now denoted in the Implementation section.
  [Reviewer 3] The reviewer suggested a note on the browser compatibility. Our system works fine with all modern browser, including Opera. Therefore we did not differentiate between the different browsers. We added a note in the text, that the user needs an updated browser to use the framework.

Case Study
----------

* The qualitative evaluation was put forth as weak point of our work, so we replaced it almost completely.
* We conducted an case study with two domain experts. Due to the high degree of expertise needed to understand the data as well as the epidemiological background it was not possible to consult more specialists-but since both of these experts play major roles in the entire study as well decide, which features and image modalities are included in future acquisition cycles, their feedback is very valuable!
* The complete section was rewritten with the reviewer feedback in mind. The first section represents the kind of case study we conduct, followed by details about the participants as well as the setup and procedure.
* For the cases we tried to highlight the user feedback when using the prototype as well as the results. At the end of each case (hypothesis-based and hypothesis-free), we added a short summary of the general user feedback.
* Subsection "Lessons Learned" goes more into detail of the expert feedback and adds some general thoughts of the experts toward the IVA approach as well, covering some aspects of the future work as well (such as more detailed segmentation masks and enhanced brushing capabilities.)

Minor
-----

* We incorporated all minor corrections proposed by the reviewers. Here are some examples:
	* Replaced "and colleagues" with "et al". where appropriate and moved citations closer to the names (for example "Dai and colleagues explored risk factors ... [10]" changes to "Dai et al. [10] explored risk factors ..."
	* Removed implementation as first class contribution in the introduction.
	* [Reviewer 3] Moved parts of the Introduction after the contribution list as suggested
	* Dropped citation of Tufte2003 "The cognitive style of powerpoint: pitching out corrupts within cheshire" for statement "Correlation does not automatically imply causation."
	* [Reviewer 3] 6.1.1 Data Preprocessing now contains information about how we exported data from SPSS and carry over data semantics.

Revisions sorted by Reviewer
============================

Summary Rating 

5 (Accept to either track: This paper is acceptable to the Conference track, and could be considered for the TVCG track after minor revisions.) 

The Summary Review 

The reviewers recommend that this paper is scored 5: "accept to either 
track". While there is slight disagreement with the reviewers' scores, 
and that there are definitely several corrections and improvements to be 
made, after discussion the reviewers are all in agreement that the paper 
should be recommended for publication at VAST, and have agreed an overall 
score of 5 for this paper. 

This paper demonstrates a good framework to help epidemiologists analyse 
their data. The tool presents several views, including a cluster view, 
bar chart and pivot table. 

The authors must address several issues within this paper to make this 
work suitable for publication at VAST 2014, as follows: 

1) Clarify the uniqueness and the novelty of your work. 
The main contributions of the paper need to be clarified, to make it 
clear as to what is important in this paper, novel and different of your 
work to others. Clarify what you are presenting here. Especially you need 
to make it clear how your work differs from Steenwijk et al’s and other 
very similar work. This should be occur in (at least) two places: 
(i) made clear in the introduction, and 
(ii) by improving the related work, to critique current work and 
position yours in relation to the related work that you mention (see R1s 
comments in particular about the related work part, but also mentioned by 
others such as R3).
Response
--------

* We reworked the related Work section completely. It now reflects on the impact of each presented publication to our work.
* The section concludes by highlighting the uniqueness of our work, compared with the presented papers.

2) Improve references. Add references as listed by R1, R2 specifically.
Response
--------

* We added the following publications as requested by the reviewer:
	* T.Lammarsch, W.Aigner, A.Bertone, S.Miksch, and A.Rind. Towards a concept how the structure of time can support the visual analytics process. In Proc. of the Int. Workshop Visual Analytics, pages 9–12, 2011.
	* P. Angelelli, S. Oeltze, C. Turkay, J. Haasz, E. Hodneland, A. Lundervold, B. Preim, and H. Hauser. Interactive visual analysis of heterogeneous cohort study data. IEEE Computer Graphics and Applications, 2014. in print.
	* M. Q. Wang Baldonado, A. Woodruff, and A. Kuchinsky. Guidelines for using multiple views in information visualization. In Proc. of the Working Conference on Advanced Visual Interfaces, pages 110–119. ACM, 2000.
	* C. Weaver. Cross-filtered views for multidimensional visual analysis. IEEE Transactions on Visualization and Computer Graphics, 16(2):192– 204, 2010.
	* J. W. Emerson, W. A. Green, B. Schloerke, J. Crowley, D. Cook, H. Hofmann, and H. Wickham. The generalized pairs plot. Journal of Computational and Graphical Statistics, 22(1):79–91, 2013.
* [Reviewer 1] We choose Baldonado's work on coordinated multiple views over the one of Roberts, since we found it fitted better for our paper.
* [Reviewer 2] We decided against including Intelligent visualization and exploration of time-oriented data of multiple patients of Klimov et al.. It's major focus in on analyzing time-oriented data and the efficient selection of subject groups sharing a certain condition and tracking it over time. It relies heavily on hypothesis based data analysis. Since we ran out of space, we did not include this work, because we cover publication based on the time factor and explained the difference of our approach on these works.

3) Add a section on Design (see R1) that describes what design 
decisions you made, what the requirements of the tool are, how the layout 
was designed etc. why on the web, and also include a figure showing the 
complete design (see R2).
Response
--------

* Section `5 System Design and Implementation` now describes detailed each part of the system, how it was designed and also argues, why we made certain design decisions. These decisions are also supported by expert feedback.
* Fig. 3 shows the complete design as requested. Fig. 4 shows the system with opened correlation matrix view.

4) Add an explicit case study, that demonstrates the system and runs 
through a scenario (see R1 and R3 in particular). Overall the reviewers 
felt that a more detailed evaluation of this work would be very 
beneficial and would improve the quality of this publication. (ie., 
Ideally we would want to see an improvement of the evaluation, with more 
details of how the tool was evaluated, by whom, how it was evaluated (its 
method) and what were the concrete outcomes.) However while this is an 
ideal case, we understand that this may not be possible in the time given 
for presentation at VAST. Therefore, we require that the details of the 
evaluation are improved, and that a case study is added that carefully 
runs through a scenario and demonstrates the tool and it's capability and 
uniqueness. Therefore the corrections for this part are: 
(i) include more details to the current evaluation, e.g., some more 
quotes of the experts, more discussion over how, why and who was involved 
in the prototype activities (see R4) 
(ii) add a case study, that details explicitly what a user is doing, 
and with supported figures.
Response
--------

* The qualitative evaluation was put forth as weak point of our work, so we replaced it almost completely.
* We conducted an case study with two domain experts. Due to the high degree of expertise needed to understand the data as well as the epidemiological background it was not possible to consult more specialists-but since both of these experts play major roles in the entire study as well decide, which features and image modalities are included in future acquisition cycles, their feedback is very valuable!
* The complete section was rewritten with the reviewer feedback in mind. The first section represents the kind of case study we conduct, followed by details about the participants as well as the setup and procedure.
* For the cases we tried to highlight the user feedback when using the prototype as well as the results. At the end of each case (hypothesis-based and hypothesis-free), we added a short summary of the general user feedback.
* Subsection "Lessons Learned" goes more into detail of the expert feedback and adds some general thoughts of the experts toward the IVA approach as well, covering some aspects of the future work as well (such as more detailed segmentation masks and enhanced brushing capabilities.)

5). Improve the abstract focusing on what, why etc. (see R2, R3 etc)
* The abstract was completely rewritten with focus on the reviewer comments.

6) Make the minor corrections that are detailed in the reviews. 
(Especially R1 has a long detailed list that must be achieved; but the 
other reviewers also have corrections).
Response
--------

* All minor corrections have been taken into account. More extensive corrections are commented in the following sections. We also commented on very few corrections, on which we disagree.

----------------------------------------------------------------

Primary Reviewer
================

[...]

Weaknesses: 
There are several aspects of the paper that could be improved. 
(1) The related work section includes merely a set of related tools. I would have liked to see a more comprehensive section that discusses the previous related work in more detail and describes why they are important and relevant to this work and how your work differs or improves upon theirs.
Response
--------

* We reworked the related Work section completely. It now reflects on the impact of each presented publication to our work.
* The section concludes by highlighting the uniqueness of our work, compared with the presented papers. We also added the following publications as requested by the reviewer:
	* T.Lammarsch, W.Aigner, A.Bertone, S.Miksch, and A.Rind. Towards a concept how the structure of time can support the visual analytics process. In Proc. of the Int. Workshop Visual Analytics, pages 9–12, 2011.
	* P. Angelelli, S. Oeltze, C. Turkay, J. Haasz, E. Hodneland, A. Lundervold, B. Preim, and H. Hauser. Interactive visual analysis of heterogeneous cohort study data. IEEE Computer Graphics and Applications, 2014. in print.
	* M. Q. Wang Baldonado, A. Woodruff, and A. Kuchinsky. Guidelines for using multiple views in information visualization. In Proc. of the Working Conference on Advanced Visual Interfaces, pages 110–119. ACM, 2000.
	* C. Weaver. Cross-filtered views for multidimensional visual analysis. IEEE Transactions on Visualization and Computer Graphics, 16(2):192– 204, 2010.
	* J. W. Emerson, W. A. Green, B. Schloerke, J. Crowley, D. Cook, H. Hofmann, and H. Wickham. The generalized pairs plot. Journal of Computational and Graphical Statistics, 22(1):79–91, 2013.

(2) Another weakness is on the data analysis; while there is information about the data within the text (including 2.2, 4.1, and 5.2) I would like to see a section that focuses on the data and the challenges thereof.
Response
--------

* We extended Section 2.2 with general challenges of epidemiological data. They lie in the heterogeneity, incompleteness, subject number and in the processing of associated medical image data.
* The data set used for the qualitative evaluation is discussed in more detail in Section 6.1, denoting the number of subjects, number of variables and associated problems.

(3) There is little detail about the design, and how it was decided to create this particular design; what interaction was made with the users, how did they influence this design? 
Response
--------

* Section `5 System Design and Implementation` now describes detailed each part of the system, how it was designed and also argues, why we made certain design decisions. These decisions are also supported by expert feedback.

(4) the evaluation could be more detailed, and present better what the tool achieves and how a user can operate it, and what each of the views tells the user.
Response
--------

* The qualitative evaluation was put forth as weak point of our work, so we replaced it almost completely.
* We conducted an case study with two domain experts. Due to the high degree of expertise needed to understand the data as well as the epidemiological background it was not possible to consult more specialists-but since both of these experts play major roles in the entire study as well decide, which features and image modalities are included in future acquisition cycles, their feedback is very valuable!
* The complete section was rewritten with the reviewer feedback in mind. The first section represents the kind of case study we conduct, followed by details about the participants as well as the setup and procedure.
* For the cases we tried to highlight the user feedback when using the prototype as well as the results. At the end of each case (hypothesis-based and hypothesis-free), we added a short summary of the general user feedback.
* Subsection "Lessons Learned" goes more into detail of the expert feedback and adds some general thoughts of the experts toward the IVA approach as well, covering some aspects of the future work as well (such as more detailed segmentation masks and enhanced brushing capabilities.)

Importance: 
The work is important, in that exploratory tools are required in several 
domains, and epidemiology appears to be one such area where this would be 
highly relevant and suitable. The work starts to synthesize other 
research, e.g., it uses brushing and linking of multivariate data. 
However, I feel that it is unclear as to what interactive operations are 
included, what they provide and how a user would operate them. E.g., how 
is brushing used between views and what does it demonstrate?
Response
--------

* Section 5 System Design and Implementation and Fig. 3 now describe the brushing and linking facilities.

Relevance: The work presents a framework, and the implementation is made 
using web frameworks. This is a relevant implementation strategy and one 
that will definitely increase in the future. The work will interest VAST 
practitioners however I feel that there is much detail missing. I am not 
currently convinced that, in its current form, that this paper is 
publishable for VAST - however the VAST venue would be suitable, but this 
paper should be improved to be published here. 

Novelty: The work develops upon known ideas, such as coordinated multiple 
views, brushing/linking, pivot tables and multi-dimensional statistical 
analysis techniques. 

Quality: The work contains many references. But there are potentially 
some missing; e..g, the framework talks about utilizing multiple 
coordinated views (although the details of what is actually linked is 
vague) and therefore cited papers such as Baldonado's work in AVI 2000, 
or Roberts 2007 on Coordinated multiple views, or Weaver's Cross-filtered 
Views for multidimensional visual analysis 2010 should be cited. 
The paper really proposes a framework; however it was unclear how this 
was implemented into the presented system. Therefore this should be 
improved. 
Response
--------

* As described before, we included these paper into the related work section. We choose Baldonado's work on coordinated multiple views over the one of Roberts, since we found it fitted better for our paper.

Other: 
Finally the figures could be improved. I felt that it was difficult to 
understand what the figures were demonstrating - as a reader, what should 
I be looking at and noticing in the figures, what can I learn from the 
visualizations? There was no supplementary material.
Response
--------

* We revised all figures. The evaluation figures were replaced.

Corrections:
My suggestion is that the paper can be improved through clarifying the 
unique points of this work, and what is novel in comparison with the 
related work; include a section on Design, improving the related work (as 
described above) and including a clearer and more defined analysis 
section on the epidemiological data that is used in this work. A case 
study, that demonstrates more clearly how the software is used, and 
clarification over what the images/figures are representing, and a more 
comprehensive evaluation of how the users have integrated the software, 
or used it, in their current work, would also benefit this work 
substantially.
Response
--------

* These summarizing suggestions are covered in prior points

Minor corrections: 

Response
--------

* All minor correction points were addressed without exception. On some, we added an explanation.


* line 2: Cohort studies comprise heterogenous variables > Cohort 
studies comprise of heterogenous variables 

* The abstract contains two paragraphs; I suggest that the first 
paragraph is removed (this is information that should be included in the 
introduction). 

* Sec 1: Para 2, thousands of persons randomly > thousands of people 
who are randomly 

* the sentence: "Due to this random selection, the majority of the 
cohort does not suffer from a specific health problem." not sure if this 
logic is absolutely true! how can a cohort suffer from a 'selection',. 
Suggest a re-wording here 

* I feel that the discussion/arguments and reasons for this software 
(i.e. the wording in paragraph 2 of the introduction) could be improved. 
There is a large amount of concepts here which are not well organised. 

* Sec 2.1: Following Thew and colleagues, > Following Thew et al [35], 
, the workﬂow can be characterized as follows: 
* 2.1 Statistics tools such as > Statistical tools such as 
* 2.1 "Graphic data representation is largely used to present results 
rather than gaining insight." this does not scan - don't graphical tools 
help users gain insight. 
* 2.2 Indicators for medical conditions as well as questions about a 
subject's lifestyle are also often dichotomous > it's better to have the 
also earlier, it currently implies that the previous sentence was talking 
about dichotomous data. 
* 2.2 , on the initial software and hardware version during a 
longitudinal study > reword 
* 3. "the strength of different visualization techniques needs to be 
combined", combined how? You cite some linking papers, but how are the 
data correlated between views?
	* RESPONSE: this point was removed. View linking is covered in the design section.
* Their focus on hypothesis generation > specify who "Their" refers 
to 
* There are many ideas in section 2.1 and I feel that the sentences 
rather move around, so the flow of this section could be improved. 
* Put the citation closer to the name: Turkay e.g., work of Tukay et 
al. [39] is closest to ours… 
* Put citation closer: Steenwijk and colleagues > Steenwijk et al. 
[34], and there are several examples of this in the remaining text. 
* when you write "This can be achieved by using data wrangling tools 
such as OpenRefine4", did you actually use OpenRefine, 
	* RESPONSE: We removed the reference to OpenRefine, since we did not use it and we felt it was not that important.
* 4.3 and reflect routines of epidemiologists in order to be > and 
reflect the routines that epidemiologists take, in order… 
* 4.3.1 "the medical image data are directly incorporated … for each 
manifestation Fig 3."; I'm not sure what you mean by "image data", as 
there are no images on the figure. 
* 5.1 We divide the data set in image and non-image data. > We divide 
the data set into image and non-image data. 
* also, I was unsure what type of image data you had - a better 
description and analysis of the data would help here.
	* RESPONSE: This is now covered in the Application Section under "The Lumber Spine Data Set"
* 5.4.1 the following sentence is difficult to parse: Another 
multivariate analysis using a pivot table set gender and employment 
status in relation to clustering affiliation, showing that cluster 8 
contains mostly women and also has a larger 
* Fig 7; it is difficult to know what to look at in the picture - make 
it clear what the reader should focus upon, or compare. The change 
between red and blue colours is also unclear. Therefore, clarify what 
this is showing.

----------------------------------------------------------------

Reviewer 2
==========

Overall Rating 

5 (Accept to either track: I would argue strongly for accepting this paper to the Conference track, and would not deplore a decision to have it in the TVCG track.) 

Topic Classification 

Applications of Visual Analysis Techniques 

Best Paper Award 

No 

Contribution to the field of Visual Analytics 

The paper presents a design study using multi-variate abstract data, 
shapes extracted from image data, and clustering results. It presents a 
workflow, a design of a tool, and usage scenarios. 
The contribution of design study papers is often subject of disagreement. 
Therefore I will base my review on the 3 research contributions described 
by Sedlmair et al. [2012, p. 2432]: 
- Problem characterization and abstraction: This is performed well using 
abstractions from the IVA framework [Oeltze et al. 2012]. 
- Validated visualization design: The visualization tool is described 
well. The validation are two usage scenarios and qualitative expert 
feedback. While these are sufficient, they need to be presented in more 
detail (see technical soundness below). 
- Reflection: The paper ends quite abruptly and misses the opportunity to 
draw lessons learnt and generalize guidelines. (This might be subject for 
follow-up work.) 
Therefore, I would argue this is acceptable with minor revisions though 
not a strong contribution yet. 

Expertise 

3 (Knowledgeable) 

The Review 

=== What are its strengths? === 

- Good insights into the domain and workflows. 
- Abstraction using the IVA framework. 
- Foucs on statistical soundness (e.g. overfitting, correlation not 
causation). 

=== What are its weaknesses? === 

- Details missing in reporting the validation.
Response
--------

* The qualitative evaluation was put forth as weak point of our work, so we replaced it almost completely.
* We conducted an case study with two domain experts. Due to the high degree of expertise needed to understand the data as well as the epidemiological background it was not possible to consult more specialists-but since both of these experts play major roles in the entire study as well decide, which features and image modalities are included in future acquisition cycles, their feedback is very valuable!
* The complete section was rewritten with the reviewer feedback in mind. The first section represents the kind of case study we conduct, followed by details about the participants as well as the setup and procedure.
* For the cases we tried to highlight the user feedback when using the prototype as well as the results. At the end of each case (hypothesis-based and hypothesis-free), we added a short summary of the general user feedback.
* Subsection "Lessons Learned" goes more into detail of the expert feedback and adds some general thoughts of the experts toward the IVA approach as well, covering some aspects of the future work as well (such as more detailed segmentation masks and enhanced brushing capabilities.)

- More details on interaction: How does one initiate clustering, derive 
features, or take over features from the contingency matrix. 
Response
--------

* Section `5 System Design and Implementation` now describes detailed each part of the system, how it was designed and also argues, why we made certain design decisions. These decisions are also supported by expert feedback.
	* Details about initiation of cluster are also covered
	* The new Application Section now also covers the use of the contingency matrix

=== Is this work relevant for VAST? If not, what other venues would be 
appropriate? === 

I would argue that the work is a relevant design study in Visual 
Analytics, though I would also review it as a similarly rated 
contribution at IEEE InfoVis and IEEE SciVis. 

=== Is related work adequately referenced and if not what citations 
should be added? === 

The paper references a good selection of literature. However, some 
references are wrong or incomplete (see revisions required). In addition, 
the following paper are related to the presented topics: 

- I would suggest to also cite the original Generalized Pairs Plot and 
not only the adaptation as GPLOMS [21]: J. W. Emerson and W. A. Green. 
gpairs: The Generalized Pairs Plot, 2012. R package version 1.1. 
- A related process model for Visual Analytics that focuses on hypotheses 
and models: T. Lammarsch, W. Aigner, A. Bertone, S. Miksch, and A. Rind, 
“Towards a Concept how the Structure of Time can Support the Visual 
Analytics Process,” in Proceedings of International Workshop on Visual 
Analytics (EuroVA 2011) in conjunction with EuroVis 2011, Goslar, 
Germany, 2011, pp. 9–12. 
- VISITORS is related work in visualization of medical variables of 
cohorts: D. Klimov, Y. Shahar, and M. Taieb-Maimon, “Intelligent 
visualization and exploration of time-oriented data of multiple 
patients,” Artificial Intelligence in Medicine, vol. 49, no. 1, pp. 
11–31, May 2010. 
- another, forthcoming related paper: P. Angelelli, S. Oeltze, C. Turkay, 
J. Haasz, E. Hodneland, A. Lundervold, A. Lundervold, B. Preim, and H. 
Hauser, “Interactive Visual Analysis of Heterogeneous Cohort Study 
Data,” IEEE Computer Graphics and Applications, vol. Early Access 
Online, 2014.
Response
--------

* The publications are added with one exception
	* We decided against including Intelligent visualization and exploration of time-oriented data of multiple patients of Klimov et al.. It's major focus in on analyzing time-oriented data and the efficient selection of subject groups sharing a certain condition and tracking it over time. It relies heavily on hypothesis based data analysis. Since we ran out of space, we did not include this work, because we cover publication based on the time factor and explained the difference of our approach on these works.

=== Are the technical results sound? Are the methods and techniques 
described in adequate detail? === 

The visualization design and technical implementation appear to be sound. 
The validation method needs to be described in more detail.
- It remains unclear who performed the analysis reported in Sect. 5.4.1 
and 5.4.2 - the developers or domain experts. From the textual clues I 
assumed it is a usage scenario as described by Sedlmair et al. [2012] and 
Isenberg et al. [2013]. cp. "Doing a real case study but not reporting on 
the details leaves the reader questioning the approach and eventually 
decreases the perceived strength of an evaluation." [Isenberg et al., 
2013, p. 2823] 
- Also the qualitative feedback in Sect.5.4.3 needs to be expanded: How 
many experts? Years of expertise? More details on the results, possibly 
direct quotes. 
Of course results from a larger case study performed by domain experts, 
possibly MILCS [Shneiderman & Plaisant, 2006], would be beneficial but I 
agree with Isenberg et al. [2013] that this is not a necessary 
requirement.
Response
--------

* The Application part and qualitative evaluation was rewritten as described in a previous point.

=== Is the exposition clear? How could the structure or style of the 
presentation be improved? ===

cp. revisions required below 

=== Should anything be deleted or condensed from the writeup? === 

- The abstract should be formulated more concisely and focus on What? 
Why? How? What follows?
Response
--------

* The abstract was completely rewritten with this feedback in mind.

- Technical details of implementation and data preprocessing can be 
shortened.
Response
--------

* Since another review suggested more detail on the implementation, we decided to to leave it as it is include the minor corrections to it.

=== Is the length of the paper appropriate for its contribution? Is it 
too long or too short? === 

The length is appropriate, though an extra half page would best be 
dedicated to more details on validation and additional figures. 

=== Are the figures informative? === 

- The figures are informative and well captioned. 
- Figure 1.b might fit better to Figure 2. 
- A figure showing the complete design (with adjacency matrix) is 
missing. 
- In the caption of Figure 3 the spine shape is not mentioned.
Response
--------

* Figures were revised with this feedback in mind. Figure 3 (left) shows the complete framework and Figure 4 the framework with opened correlation matrix view.

=== Is the (optional) supplementary material helpful? === 

not applicable 

=== Minor and Spelling Revisions Required ===
Response
--------

* All corrections are included in the publication

- The abstract should mention the validation described. 
- Introduction: The sentence on modern web technology ("The easy ...") is 
confusing and appears misplaced. 
- I would not regard the implementation as a 1st class contribution that 
receives a bullet in this list. 
- I propose to move the 2 sentences on validation ("We applied ...") 
after the bullet list. 
- Background: The discussion on groups and confounders reminded me of 
Simpson's paradox, which makes a convincing case for careful data 
analysis. Is that related to the problem at hand? 
- The order of Figure 2 and Figure 3 should be fixed. 
- In Figure 3 left there are 4 body size groups but on the right and in 
the small image above the arrow there are only 3 groups. 
Response
--------

* This is due to the the mapping on gender, the size-group 139-153.5 cm is only populated by women, while 182.5-197 contains only men.

- Figure 3 mentions the age parameter, where in fact the gender parameter 
is dropped. 
- Sect. 4.3.1: The mapping of the adjacency matrix is to color brightness 
not to color hue(!). 
- Sect. 5.4.3: It is strange why a Tufte book on Powerpoint is referenced 
for correlation/causation. I would regard this either as a commonly known 
fact or reference some Statistics/scientific methodology publication. 
- References [20] and [30] lack page numbers. 
- Reference [24] lacks publication details such as booktitle, venue, 
pages. 
- Reference [28] appeared in 2012 -- the year when IEEE VIS took place in 
Seattle(!). 
- Reference [38] I'm not aware of a 2nd volume of The visual display of 
quantitative data and AFAIK Tufte is the single author. 
- I'd suggest to remove the keyword "Visualization System and Toolkit 
Design".

----------------------------------------------------------------

Reviewer 3
----------

Title: Interactive Visual Analysis of Image-Centric Cohort Study Data 

Reviewer: external 

Overall Rating 

4 (Merit a presentation: I would argue for accepting this paper to the Conference track.) 

Topic Classification 

Applications of Visual Analysis Techniques 

Best Paper Award 

No 

Contribution to the field of Visual Analytics 

The paper describes the integration of visual analytics into an 
epidemiological workflow that uses different visualisation approaches to 
previous work. The user can examine a heterogeneous dataset for 
correlated features, or starting with their own hypothesis, find related 
features that support or contradict that hypothesis. 

Expertise 

2 (Passing Knowledge) 

The Review 

Summary: The paper describes the integration of visual analytic processes 
into the workflow of epidemiological studies where data can include 
medical images and continuous and categorical variables. They explain in 
this particular field, epidemiology, that visualisation usually occurs 
after the analysis (to show results) and is not used as an aid during the 
analysis, and that this is where their contribution lies. 

What the prior work section needs at the end is a paragraph stating how 
their work differs from the work they summarise i.e. it uses more 
non-image data than Turkay and uses different visualisations, and more 
importantly differentiation from Steenwijk et al’s very similar work 
(saying they use a different meaning for the word “cohort” does not 
seem justification enough, given the large overlap), only then can we be 
sure there is a novel contribution here.
Response
--------

* We reworked the related Work section completely. It now reflects on the impact of each presented publication to our work.
* The section concludes by highlighting the uniqueness of our work, compared with the presented papers.
* We added the following publications:
	* T.Lammarsch, W.Aigner, A.Bertone, S.Miksch, and A.Rind. Towards a concept how the structure of time can support the visual analytics process. In Proc. of the Int. Workshop Visual Analytics, pages 9–12, 2011.
	* P. Angelelli, S. Oeltze, C. Turkay, J. Haasz, E. Hodneland, A. Lundervold, B. Preim, and H. Hauser. Interactive visual analysis of heterogeneous cohort study data. IEEE Computer Graphics and Applications, 2014. in print.
	* M. Q. Wang Baldonado, A. Woodruff, and A. Kuchinsky. Guidelines for using multiple views in information visualization. In Proc. of the Working Conference on Advanced Visual Interfaces, pages 110–119. ACM, 2000.
	* C. Weaver. Cross-filtered views for multidimensional visual analysis. IEEE Transactions on Visualization and Computer Graphics, 16(2):192– 204, 2010.
	* J. W. Emerson, W. A. Green, B. Schloerke, J. Crowley, D. Cook, H. Hofmann, and H. Wickham. The generalized pairs plot. Journal of Computational and Graphical Statistics, 22(1):79–91, 2013.

The work is certainly relevant for VAST as it covers the integration of a 
visual analytic process into an existing real-world workflow. The paper 
is generally well written (with a couple of minor issues pointed out 
below) 

The technical background to the work is explained adequately (4.4) but I 
have added a comment below for one particular point. And whether it 
should count as a contribution in itself is debatable, many if not most 
visualisation systems now seem to be web-based. 

I feel the section on the Automated Feature Suggestion could be expanded, 
it seems to be one of the most visual pieces of the work and shows 
statistical relationships between all the features, but after a quick 
discussion of the statistic employed it is not mentioned again (and 
Figure 4 is only mentioned in passing in association with Figure 3). This 
would seem to be a major part of the work, but is also missing from the 
example given later in Section 5.
Response
--------

* The part on automated feature suggestion is as part of the new design section discussed in more detail.
* As part of the new evaluation, the contingency matrix and contingency pane is also included and worked very well!

Specific Comments:

Response
--------

* All points were addressed without exception. On some, we added an explanation.

In the abstract, “The presented concept are applied expert-guided” 
doesn’t make sense, should it be “… applied by experts”? 

Typo; Section 4, 1st para: “compensate its weaknesses”
“compensate for its weaknesses” 

4.1. The authors talk of exporting data from packages such as SPSS to 
formats like CSV and JSON. How do they ensure the semantics of the data 
is carried over? i.e. for a category of ordinal values such as say 
“Phd”, “Msc”, “Bsc” how is that ordering kept or do they not 
deal with such types of data? I mention it as it’s been a problem of 
mine in the past when exporting to CSV etc. 
Response
--------

* 6.1.1 Data Preprocessing now contains information about how we exported data from SPSS while and carry over data semantics.

4.2 The second and third sentences read like they’ve been split apart, 
as the third sentence “A feature selection from a shape-based 
clustering, which creates shape groups” makes no sense on its own. 

In 4.3.1. state specifically which parts (sidebar, canvas, pivot table, 
contingency view) belong to which figure. I spent a while searching for 
the contingency view in Figure 3 before turning the page to see it was in 
Figure 4. 

In the Pivot Table section, there’s this sentence: “Epidemiologists 
are used to process groups based on table representations.” Does this 
mean they are employed to process groups, or should it be 
“processing”, as in they are familiar with dealing with data 
presented in pivot tables?
Response
--------

Reworded this to `Epidemiologists are used to perform multivariate analysis of groups based on table representations`

4.4. the R “Shiny” library can be used to communicate between R and a 
web browser, by using its message passing functionality (and there are 
other R packages such as Rook that claim to do similarly). Whether it 
integrates well with all the other back-end stuff (NodeJS etc) is another 
issue though. 
Response
--------

* This is correct! The R shiny package does allow to use R code on the web, but in a very closed manner, you have to use their system (and ideally the RStudio IDE) to make this work. If you are interested in usages of R in a web context outside of Shiny, you can have a look at (RServe)[http://rforge.net/Rserve/]. I made an interface a year ago for RServe to Node.js, but its more a proof of concept thing (https://github.com/Powernap/rserve-js-Interface). For this work it was way easier though to implement the statistics algorithms from scratch, eliminating the need to work with another local server, like RServe.
    * These possibilities are now denoted in the Implementation section.

4.4. Mention that the browser needs to support these technologies and 
what this could mean (i.e. no Internet Explorer before a certain 
version). For instance, out the box, the latest Chrome version will run 
the three.js examples, but Opera (based on the same WebKit engine) 
won’t. 
Response
--------

* Our system works fine with all modern browser, including Opera. Therefore we did not differentiate between the different browsers. We added a note in the text, that the user needs an updated browser to use the framework.

5. The example given is based on a single data set. While I understand 
it’s difficult to acquire such large real-world data sets, and the 
ethical agreements and hoops to jump through, it would have been good to 
have a data set that allowed the demonstration of the full functionality 
of the system i.e. made use of the contingency matrix view as well.
Response
--------

* We extended the analysis to more subjects. We now cover 6.753 subjects and 2.440 segmented lumbar spine shapes. This allows for more statistical resilient results.
* As the epidemiologists are very enthusiastic about the work, there are currently a few applications for new data sets. Unfortunately, these processes take very long and most likely have to happen in an iterative way. But it demonstrates well, that epidemiologists are really interested in such systems
* The new Application chapter covers use of the contingency matrix as well!

Also, in places in the example given in Section 5 it is difficult to tell 
whether the actions being described are what the system could do, or what 
the experts actually did do (through the guidance of the developers). 

Also, doesn’t the discretisation of continuous data into a set global 
number of categories risk over-fitting the data, or at least arbitrarily 
forcing it into unnatural categories?
Response
--------

* Both points are now addressed in the application section

Minor: have the references follow on from the end of section 6.(not a new 
page) 

In summary I would say this paper would need three things to be accepted, 
which maybe possible in the turn-around for this conference, (but 
certainly for next year). They need to more clearly delineate its 
differences to the previous work in the field, expand the section on the 
contingency matrix, and describe an example scenario (or scenarios) where 
all parts of the system (including said matrix) are shown to their 
advantage. If they can do this I would argue for acceptance as a 
conference-only presentation. 
Response
--------

* These summarizing suggestions are covered in prior points

----------------------------------------------------------------

Secondary Reviewer
==================

Title: Interactive Visual Analysis of Image-Centric Cohort Study Data 

Reviewer: secondary 

Overall Rating 

7 (<b>Definite accept (TVCG track):</b> I would argue strongly for accepting this paper.) 

Topic Classification 

Applications of Visual Analysis Techniques 

Best Paper Award 

Yes 

Contribution to the field of Visual Analytics 

First off, after reading quite a few submissions this year, it was a 
pleasure to review this paper. This is an elegant, professional, 
polished paper that tells the "story" of IVA with just the right amount 
of detail and illustration. The authors do a great job describing the 
design space, contextualize their work in relation to similar efforts, 
and clearly explain how the visualizations and interaction model supports 
exploratory analysis of epidemiological data. I liked the mouseover 
interactions for visual exploration of the adjacency matrix - I'd like 
that functionality for some of the gnarly data I deal with. I also 
liked the section on implementation, including the pros and cons of using 
open web standards for tool development, as well as the comparison of 
hypothesis-free and hypothesis-directed data analysis. The paper could 
be strengthened with more detail about developer interactions with domain 
experts/potential users during the design and prototype activities.
Response
--------

* We now show how expert feedback influenced design decisions in the new section `5 System Design and Implementation`
* The new application and evaluation section now describes detailed, how the evaluation was carried out and what we learned from their feedback.

Expertise 

2 (Passing Knowledge) 

The Review 

STRENGTHS. This submission is refreshingly well written. It's a very 
professional, polished discussion of the team's work in designing, 
developing, and implementing a system for visual interaction with 
epidemiological data. 

WEAKNESSES. Few. The paper would be strengthened by including more 
detail about the team's interactions with the domain experts; i.e., the 
expert community who informed their discussion of the epidemiological 
workflow described in section 2.1 and their prototype evaluation goals, 
metrics, and findings, which get only cursory treatment in section 5.4.3. 
Response
--------

* See previous response.

DISCUSSION. Kudos to the authors for writing a great paper. These 
authors demonstrate excellent expository skills and appreciate the 
importance of clarity when presenting the technical details of a 
scientific visualization domain for a diverse audience. If only all 
papers were this well written! 

I don't have many comments about the content of the paper; I thought it 
covered quite a broad range of themes and topics with considerable skill. 
However, there wasn't much information about interactions with the user 
community. How did you engage domain experts during your design, 
implementation and evaluation activities? For that matter, how did you 
identify your user community? The lack of detail was particularly 
apparent in Section 5, where there are glancing references to 
interactions with domain experts, but not much detail about the nature 
nor characteristics of those interactions. This is a common problem 
with Vis papers and the authors could strengthen their already solid work 
with more detail about the prototype evaluation - in fact, they've got 
plenty of space to work this in. 

So: when interacting with users at different points in the process…. 
What were the goals? How did you select domain experts to participate? 
Were these the same domain experts that provided input for the workflow 
mapping and characterization? Was the demonstration discussed in section 
5 focused on face validity, or did you have other evaluation goals? How 
did you gather and analyze data about the user experience (if you did)? 

Please note: It's fine NOT to have done a detailed evaluation, but it'd 
be great to say that clearly, then discuss the goals of the user feedback 
process. Generally speaking, more discussion about how, why, and who was 
involved in prototype feedback activities - and how these activities 
relate to earlier design-related interactions/requirements analysis - 
would make an already strong paper a real standout.
Response
--------

* The qualitative evaluation was put forth as weak point of our work, so we replaced it almost completely.
* We conducted an case study with two domain experts. Due to the high degree of expertise needed to understand the data as well as the epidemiological background it was not possible to consult more specialists-but since both of these experts play major roles in the entire study as well decide, which features and image modalities are included in future acquisition cycles, their feedback is very valuable!
* The complete section was rewritten with the reviewer feedback in mind. The first section represents the kind of case study we conduct, followed by details about the participants as well as the setup and procedure.
* For the cases we tried to highlight the user feedback when using the prototype as well as the results. At the end of each case (hypothesis-based and hypothesis-free), we added a short summary of the general user feedback.
* Subsection "Lessons Learned" goes more into detail of the expert feedback and adds some general thoughts of the experts toward the IVA approach as well, covering some aspects of the future work as well (such as more detailed segmentation masks and enhanced brushing capabilities.)