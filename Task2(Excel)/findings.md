Task 2: Forensic Technology — Pay Equality Analysis (Excel)

What I learned: How to use Excel formulas to classify and analyze data at large scale.

What the task involved:
1.Analyzing an Equality Score dataset across factories and job roles
2.Classifying each score into a pay-equality category using a formula

The data: Daikibo's Forensic Tech team generated an Excel file with 3 columns — Factory, Job Role, and Equality Score.

The goal: Add a 4th column classifying each Equality Score into one of three categories:

Fair: between -10 and +10
Unfair: below -10 or above +10
Highly Discriminative: below -20 or above +20

What I did: Created a calculated 4th column ("Equality class") using a nested IF/OR formula:
=IF(OR(C2<-20,C2>20),"highly discriminative",IF(OR(C2<-10,C2>10),"unfair","fair"))
This checks the most extreme cases first (highly discriminative), then unfair, then defaults to fair.

What I found:
1.Several C-Level, VP, Director, and Sr. Manager roles across factories (especially Daikibo Factory Meiyo and Seiko) fell into the "highly discriminative" category, with scores as low as -26.
2.Mid-level roles like Sr. Manager, Manager, and Jr. Manager frequently landed in the "unfair" range.
Engineering and operational roles (Sr. Engineer, Engineer, Jr. Engineer, Machine Operator) were mostly classified as "fair," staying within ±10.