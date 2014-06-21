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

Abstract
--------

* [Reviewer 3] The abstract was shortened as requested by Reviewer 3, moving parts into the introduction.

Epidemiological Data
--------------------

* [Reviewer 1] Reviewer 1 requested more details about the data and the challenges thereof.
	* We enhanced Section '2.2 Epidemiological Data' with challenges associated with epidemiological data.
	* Section '6.1 The Lumbar Spine Data Set' now describes the data in more detail.

Fig. 3
------

* [Reviewer 2] Reviewer 2 noted that "In Figure 3 left there are 4 body size groups but on the right and in  the small image above the arrow there are only 3 groups." This is due to the the mapping on gender, the size-group 139-153.5 cm is only populated by women, while 182.5-197 contains only men.

Background
----------

* [Reviewer 2] Information about `Simpsons Paradox` added. Reviewer 2 pointed out a possible relation between confounders and Simpsons Paradox. The Reviewer is right, since Simpsons Paradox is a very extreme case of a confounder (http://www.bmj.com/content/309/6967/1480).

Implementation
--------------

* Due to the lack of space we did not expand the `Implementation` section. Also Reviewer 2 and Reviewer 1 made contrary statements about whether the section should be extended or shortened.
* [Reviewer 3] The R shiny package does allow to use R code on the web, but in a very closed manner, you have to use their System (and ideally the RStudio IDE) to make this work. If you are interested in usages of R in a web context outside of Shiny, you can have a look at (RServe)[http://rforge.net/Rserve/]. I made an interface a year ago for RServe to Node.js, but its more a proof of concept thing (https://github.com/Powernap/rserve-js-Interface). For this work it was way easier though to implement the statistics algorithms from scratch, eliminating the need to work with another local server, like RServe.
    * These possibilities are now denoted in the Implementation section.
  [Reviewer 3] The reviewer suggested a note on the browser compatibility. Our system works fine with all modern browser, including Opera. Therefore we did not differentiate between the different browsers. We added a note in the text, that the user needs an updated browser to use the framework.

Case Study
----------

* We conducted an case study with two domain experts. Due to the high degree of expertise needed to understand the data as well as the epidemiological background it was not possible to consult more specialists-but since both of these experts play major roles in the entire study as well decide, which features and image modalities are included in future acquisition cycles, their feedback is very valuable!
* The complete section was rewritten with the reviewer feedback in mind. The first section represents the kind of case study we conduct, followed by details about the participants as well as the setup and procedure.
* For the cases we tried to highlight the user feedback when using the prototype as well as the results. At the end of each case (hypothesis-based and hypothesis-free), we added a short summary of the general user feedback.
* Subsection "Lessons Learned" goes more into detail of the expert feedback and adds some general thoughts of the experts toward the IVA approach as well, covering some aspects of the future work as well (such as more detailed segmentation masks and enhanced brushing capabilities.)

Minor
-----

* Replaced "and colleagues" with "et al". where appropriate and moved citations closer to the names (for example "Dai and colleagues explored risk factors ... [10]" changes to "Dai et al. [10] explored risk factors ..."
* Removed implementation as first class contribution in the introduction.
* [Reviewer 3] Moved parts of the Introduction after the contribution list as suggested
* Dropped citation of Tufte2003 "The cognitive style of powerpoint: pitching out corrupts within cheshire" for statement "Correlation does not automatically imply causation."