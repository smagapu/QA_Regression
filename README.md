QA_Regression
=============

Regressing the Chesea API

All the inputs should be before the expected results and should start with input_****
ex: input_url
All the expected results should be defined after the inputs and shoul begin with expected_****
ex: expected_width
Note: All the sub parameters ex: all the exif parameters should be in the following format.
expected_exif[color], expected_focal_point[width].

Example:
input_uri,input_owner,expected_width,expected_face_count, expected_focal_point[width],expected_focal_point[height] \n http://thm-usa.dnsalias.com/website/photogallery/thecrew.jpg,timmah,3264,5, 1632, 1224
http://thm-usa.dnsalias.com/website/photogallery/exif_gps.jpg,jimmah,3264,1, 1632, 1224
http://thm-usa.dnsalias.com/website/photogallery/exif.jpg,jimmmaah,500,0, 250, 142
https://lh5.googleusercontent.com/-tK8tC8todI4/T5Ynm74DC8I/AAAAAAAAEWw/nsTZ7IxAAA0/s628/IMG_0247.JPG,Magapu,628,2, 314, 142

--Whenever the CSV file and the Development code get updated this regression suite triggers automatically
and throws the results against the expected output in the CSV file.
--The result can found at "Rspec report" under each build in  http://16.86.193.109:51526/job/Newcastle_QA
--The failed cases are displayed in RED with the result and the passed cases are displayed in GREEN