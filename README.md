# spy.pet checker

Crawls your discord servers and a list of known spy.pet compromised discord server if you are in any spy.pet discord servers it returns the user id of the spy.pet account.

> [!IMPORTANT]
> spy.pet changed the api and is now blocking attempts by this script to verify user id info. I will update this script once the changes to the API are understood.

## Usage

* clone the repo: `git clone https://github.com/aetaric/spy.pet_checker && cd spy.pet_checker`
* setup virtualenv: `virtualenv venv && source venv/bin/activate`
* install requirements: `pip3 install -r requirements.txt`
* edit line 19 and 20 to have your [discord application](https://discord.com/developers/applications)'s Client ID and Client Secret
* run the app and authorize: `python3 login.py`


## Setting up a new discord application

* Visit https://discord.com/developers/applications and create a new application.
* click the oauth tab on the left
* scroll to `Redirects` and add a redirect
* set the redirect value to `http://127.0.0.1:5000/callback`
* save the application
* click reset secret at the top to get a new secret
