# MKDEV


McKnight DE 
Pipeline Analysis READ ME

Author: Daniela Torre
Date: Sept 24, 2015

Date drafted: Sept 2015 (from MK15 report)

Date revised: Sept 2015

Datasets pulled in: MK15-cleandata-studentlevelanalysis.dta 


NOTE: We're using the data that was cleaned for the MK15 report -- no need to re-clean it

Datasets produced: ${newdata}all program schools clean.dta


Purpose (a broad overview of what the code does):

	1) Append clean data files from each district, dropping only to students/ schools/ variables necessary for analysis
	2) Run piple line results by cohort only (combining all schools). Run by DLL and nonDLL. 
		-Want just K as denominator. 
		-Driving question: if the program is supposed to work over the course of K-3, how many kids are still in district in 3rd grade to have been in entire program
	3) Save results in a way that can be easily read
	4) Make pie charts by cohort only (combining all schools). Run by DLL and nonDLL.
	5) Make survival type charts by cohort only, by district, school and by dll status

	
	NOTE: We had a problem with the SPPS Race variable in the descriptives, wherein it was labeled the same as the other two districts but it's actually coded differently.
			The code in here already fixed that problem, so there was no effect on the results
			
	NOTE: Something is off with the 2011 and 2014 cohorts of SPMA data. I ran all graphs with and without SPMA. Going forward, we should try to get a new copy or find a better 	version of SPMA data. 
