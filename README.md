# MyFirst
My frist project on git
#Sql query to find enrollment wich is not available in fb_user_info_2 table
 $numfed1   =  "select * from candidate_details_tb WHERE enroll NOT IN(select enroll from fb_user_info_2) and sem='{$selecta[sem]}' and 
		division='{$selecta[division]}' and course='{$selecta[branch]}' and active='Y' group by enroll order by enroll";
