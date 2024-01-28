# seascape-video-assign

Tool for assigning diver operated videos (DOVs) from the Vatu-i-Ra Seascape for classroom quantitative analysis activities, packaged as a stand-alone offline html file.

For more information on the classroom activities. See _Lessons in Conservation_, **Vol. 13**, Issue 1, pp. 15-37, which is accessible via [ncep.amnh.org/linc](http://ncep.amnh.org/linc).

The html file implements (via javascript) an algorithm to randomly assign DOVs to students for quantitative analysis in the classrooms. The algorithm aims to balance the number of videos taken from each site (especially to balance the number from fished sites and tabu [= _non-fished_] sites), as well as the difficulty of analyzing the videos in the subsequent task.

The algorithm first pick out the number of videos each student is assigned from each level of difficulty, then select these at random while trying to balance the sites they come from. Then, the selected videos are randomly assigned to the students in a "column-first" manner (i.e, all students are assigned a first video before a second video is assigned), subjected to the condition that no videos are repeatedly assigned to the same students. In addition, the javascript also provides support for presenting the assignment result in html table, as well as saving the assignment in both html and csv formats.

The html file conforms to the HTML5 standard and the javascript can be executed by any browser that implements core features of the ECMAScript 2015 (a.k.a. ES6). For older browsers, down transpiling should be an option. However, it is advised to keep the source javascript non-minified for transparency sake.

Somewhat counterintuitively, a stand-alone offline html file is deemed suitable for the purpose of this tool since the browser is easily the most common piece of software found on any modern computers.
