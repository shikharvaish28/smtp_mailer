# SMTP Mailer

Send personalised mails from your domain-email to n-number of people from your terminal.

## Features

* Intentionally detailed names, so that the user would know to whom the e-mail has been sent.
  * The ```.csv``` file is read for e-mail and names of the contact. The ```.csv``` file uses it as a 2-D array.
  * Can be used with ```txt``` and other file formats too(With a minor code change).
  * Tested on Mac (Python 3.6).

## Instructions to send mails using smtp_mailer

* [smtp_mailer][1] basically needs a input source from where it can read the email address
    (which of course has video lectures).

  * Make a [virtual environment][3] for this project on your local machine and download ```smtplib``` using ```pip install smtplib``` or ```pip3 install smtplib``` (In case there are a number of python versions installed on your system).

  * Enter the details in the attributes:
    * ```SMTPserver``` : ```mail.domain.com```
    * ```sender``` : ```email@domain.com```
    * ```USERNAME``` : ```cpanel_login```
    * ```PASSWORD``` : ```cpanel_password```

  * Enter the ```Subject``` and ```body``` of the e-mail. You can decorate it using ```HTML``` tags.

  * Enter the location of the ```.csv``` file and configure the ```line``` and ```row``` as per your needs.

  * Run ```python smtp_mailer.py``` or ```python3 smtp_mailer.py``` in case you have more than one versions of python installed on your system.  
  
  * Voila! Mails must have triggered by now.
  
## Contributions

   If you want to contribute to this project, feel free to fork it and send a PR :)

## Coming Up

* [smtp_mailer][1] only supports its using terminal. Attempts are to make a GUI based app where you can upload the ```csv``` file and an interface to view the mails being triggered.

* A GUI method to input ```ID``` and ```password```

* Remove the dependency on cpanel credentials.

* Add the reciever end using POP3 client.

## Contact  

  Shoot a mail at shikarvaish@gmail.com
  
## Author

  [Shikhar Vaish][2]

[1]: https://github.com/shikharvaish28/smtp_mailer
[2]: http://shikharvaish.me
[3]: https://www.pythonforbeginners.com/basics/how-to-use-python-virtualenv/
