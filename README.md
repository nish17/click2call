# Click 2 Call

This is an example of a Click To Call application built in Python using the Nexmo Voice API. You could embed the web form on your company's website and configure the application with your sales phone number.

When customers want to talk to you they enter their name and number into the form and Nexmo will setup a call between you and the customer. First your number is called and the call is announced with the customers name, then the customers number is called and you are connected.

You can test out your own copy of this right now on heroku by clicking this button:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/nexmo-community/click2call)

This will launch the Heroku installer console. You will be asked to enter a name for your app (we need this twice) - something like "CallFred" is good.
It will also ask you to enter the number where you want callers to be connected to. Enter your number in international format without the + eg `447790900123`
It will also ask you for your Nexmo API Key and Secret and finally it will ask you to enter a country where you would like to purchase a nexmo number, For this demo the number is only used for the Caller ID.


## Running Locally
If you wish to run the application locally you can download this repo, edit the `EXAMPLE.env` file to contain your details and rename to `.env` then add your nexmo appliaciton private key to a file called `private.key`.
Install the requirements using `pip -r requirements.txt` and launch the app by running `python app.py` 
The app will launch by default on port 5000
