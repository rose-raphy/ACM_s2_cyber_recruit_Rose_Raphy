#Challenge-6

Challenge description: 3 html files- index.html, stage.html, results.html in templates(because we need to use flask), and a python file -app.py to run these html files. 

Analysis:
Basically, this challenge is like a game. We have got the expected answers in the python file and we fill it in the stages accordingly. Towards the end of the game, we get our total score including a description of what we learned. This whole game is based on NIST Response Incident Framework. 

"Noticing problem": "Detection"
"Understanding": "Analysis:"
"Stopping damage": "Containment"
"Removing bad stuff": "Eradication"
"Making normal": "Recovery"
"Learning": "Lessons Learned"

When I entered these, it did not give me the right flag. I also tried different alternatives for the above but it did not work. 

And so, i tried flag{orion_tech_secret_key}

It also didnt work. 

I checked up in console as well as in Web developer tools. There is no additional instructions to these. 

cd Downloads
python3 -m venv venv (to enable python3 in a virtual environment)
source venv/bin/activate
python app.py 
(do the stages)
