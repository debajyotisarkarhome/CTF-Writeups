# Problem : Session

'' Oh no! Geno’s email was involved in a data breach! What was his password? http://34.69.61.54:4777 ''

## Analysis

The address on visit gives a login form and upon inspecting the html source there is a comment with the login details iroh:iron. (Lame)
Well then I got stuck with useless fantasy story which populated the page. ass the name suggests session I went to inspect the site and went to network tab reloded and served with the GET requests of the html and an image. Upon checking the cookies I found there was one sessionID token (UlN7MG5seV9PbmVfczNzc2lvbl90b2szbn0) which when decoded from base64 gives the flag 
RS{0nly_One_s3ssion_tok3n}