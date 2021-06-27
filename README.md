# tesser_ocr
OCR deployment on Heroku 

# STEPS TO FOLLOW TO DEPLOY TESSERACT OCR ON HEROKU 
1. Create your free account on Heroku 
2. Once you are in your dashboard, click on new and create a new app (also name the app)
6. Download Heroku CLI and change the stack from 20 to 18 
7. to change stack, open command prompt and login to Heroku CLI using the 'heroku login' command 
8. Type heroku app to see the list of all the apps created on heroku
9. To check for the available stacks of the app 'heroku stack -a tesser-ocr' 
10. To set the stack give this command 'heroku stack:set heroku-18 -a tesser-ocr'
11. Go back to Heroku dashboard.... In the deployment method, click on Github and connect your github account 
12. You can fork the tesser_ocr repository to create your own repo
13. Type the name of the repository in heroku and connect to it
14. Add this heroku buildpack in the settings menu https://github.com/heroku/heroku-buildpack-apt
15. Also add the python buildpack in Add buildpacks option 
16. Set config vars to  KEY :- TESSDATA_PREFIX and VALUE :- ./.apt/usr/share/tesseract-ocr/4.00/tessdata 
17. Build and deploy the app and open app
