# tesser_ocr
OCR deployment on Heroku 

# STEPS TO FOLLOW TO DEPLOY TESSERACT OCR ON HEROKU 
1. Create your free account on Heroku 
2. Once you are in your dashboard, click on new and create a new app (also name the app)
3. In the deployment method, click on Github and connect your github account 
4. You can fork the tesser_ocr repository to create tour own repo
5. Type the name of the repository in heroku and connect to it
6. Download Git and Heroku CLI and change the stack from 20 to 18 
7. to change stack, login to Heroku CLI and give this command 'heroku stack:set heroku-18'
8. Add this heroku buildpack in the settings menu https://github.com/heroku/heroku-buildpack-apt
9. Set config vars to  KEY :- TESSDATA_PREFIX    and      VALUE :- ./.apt/usr/share/tesseract-ocr/4.00/tessdata 
10. Build and deploy the app and open the created link 
