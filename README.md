# coordinated-vigilance

Code for the paper titled "Ground squirrels do not have a sentinel system but instead synchronise vigilance" 
Authors: Annemarie van der Marel, Jane M. Waterman, Marta López-Darias
Corresponding author: A van der Marel, Department of Biological Sciences, University of Manitoba, Winnipeg, Canada, avdmarel@outlook.com

Data is available in csv format and all the code is in the R markdown file "coordinated vigilance.Rmd". 

DOI: 10.5281/zenodo.4694935


Key to listed abbreviated variables:
scandata 	-> all observational data (2014-2016)
scanprim8 	-> observational data recorded using Prim8 software (2015-2016)
	orderkey 	= unique id per row
	year 	 	= year of observation
	julian_date 	= day of observation (julian_date 1 = first day of field season in Feb 2014)
	dop		= unique observation session ID (d = julian day, op = observation period)
	dos		= unique scan ID (d = julian day, o = observation period, s = scanID)
	site		= site observed in (sites 1-3)
	id 		= unique squirrel ID
	sex		= 1=males, 2 = females
	age		= 1=adults, 2=subadults, 4=juveniles
	group		= primary sleeping burrow association (nighttime social group) the squirrel is part of
	time		= time of observation in 24:00 format
	duration	= time in s that squirrels perform a state behavior (only recorded with Prim8 software from 2015-2016)
	posture		= s2=sit with 2 paws on ground, s4=sit with 4 paws on ground, 
	behaviour_1:3	= the behavior the squirrel was performing, up to 3 different behaviors
	x 		= x coordinate of a squirrel location in UTM
	y 		= y coordinate of a squirrel location in UTM
	source		= whether a predator or disturbance was observed
	comments	= any notes about the observation 


df_cost	-> dataframe for the cost of perching analyses
	year		= year data collected
	id 		= unique squirrel ID
	scans.feed 	= number of scans that the squirrel was observed foraging in that year
	scans.obs.x 	= total scans the squirrels was observed that year
	propfeed	= proportion of time spent foraging (scans.feed/scans.obs.x)
	scans.perch 	= number of scans that the squirrel was observed perching in that year
	scans.obs.y 	= total scans the squirrels was observed that year (same as scans.obs.x)
	propperch	= proportion of time spent perching (scans.perch/scans.obs.y)
	avemass		= the average mass in grams of the squirrel that year
	hf		= hindfoot length in mm 
	bc		= body condition
	survival_age 	= age the squirrel survived until
	survived	= whether the squirrel survived (1) or did not survive (2) that year. 


