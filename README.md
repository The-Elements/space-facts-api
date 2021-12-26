# Space Facts API

An API that will return random facts about space.

## Credits
Special thanks to @DukeNgn

## Usage:

+ `https://space-facts-api.techgenius7777.tech/api/v1/resources/fact/all` to get all the facts at once.
+ Change `all` to parameter `?number=` to specify the number of facts you want to receive.
+ Change `all` to parameter `?index=` to specify the index of the fact you are targeting.

> Note: The project is being hosted by Heroku with free dyno; thus, there will be potential delay the first time you make a request (app went to sleep after dyno does not receive traffic in 1 hour). Please be patient, and the call will be faster next time.

## Rebuild the project:
+ Clone the repo.
+ Run `python3 -m venv .env` to create a virtual environment.
+ Run `source .env/bin/activate` to activate the virtual environment.
+ Run `pip install requirements.txt`.
+ Run `python3 app.py`.
+ App starts at port 5000 by default, but can be configured with a `.env` file. 

## Example:
+ `https://space-facts-api.techgenius7777.tech/api/v1/resources/fact?number=1` returns:
```JSON
[
    {
        "fact": "There are more stars in the universe than grains of sand on all the beaches on Earth. That's at least a billion trillion!"
    }
]
```

+ `https://dog-facts-api.herokuapp.com/api/v1/resources/dogs?number=2` returns:
```JSON
[
    {
        "fact": "The hottest planet in our solar system is Venus."
    },
    {
        "fact": "According to mathematics, white holes are possible, although as of yet we have found none."
    }
]
```
