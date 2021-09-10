# basic information needed
## how to install chome/chromedriver in ubuntu/debian 
  #### 1- chrome install 
    # you can download chrome from here https://www.google.com/chrome/
    # double click and choose install
    # note if you are using root user you will indeed need to run chrome from terminal using --no-sandbox argument
    # example:
    google-chrome --no-sandbox  

  #### 2- install chromedriver
    # you can download chromedriver from here https://chromedriver.chromium.org/downloads
    # extract chromedriver 
    # open terminal in the directory path
    # write:
    sudo chmod +x chromedriver
    sudo mv chromedriver /usr/bin/  
    # please note that chromedriver version must support the chrome version  
     
## how to install geckodriver
  #### 1- firefox install
    # is default installed in allmost all linux distrebutions so no need to manuall install
  #### 2- install geckodriver
    # you can download geckodriver from here https://github.com/mozilla/geckodriver/releases
    # extract geckodriver 
    # open terminal in the directory path and write  
    sudo chmod +x geckodriver
    sudo mv geckodriver /usr/bin/  
    # please note that geckodriver version must support the firefox version  

## how to install python3/python3-pip and requirements.txt
  #### install python packages
    # in terminal write 
    sudo apt install python3 python3-pip
    # in the code directory open terminal and write
    pip3 install requirements.txt
    # to run python code write
    python file.py 
    # if python not working and package is installed use
    python3 file.py
    # where file is the target python main file to run
    # if there is arguments need to be passed you will write
    python3 file.py arguments
    # example: run django server for all IPs on port 5000
    python3 manage.py runserver 0.0.0.0:5000
    # to run django with certificate run the following command
    python manage.py runsslserver --certificate pathtocertificate.crt --key pathtokey.key 0.0.0.0:5000
