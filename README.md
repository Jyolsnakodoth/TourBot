# TourBot
Chatbot using RASA for tourism industry

Create a new folder for chatbot and create a new virtual environment by following steps

* python3 -m venv ./venv

* source ./venv/bin/activate

Upgrade the pip to latest form and Install Rasa open-source with the below commands

* pip3 install -U pip

* pip install rasa[spacy]

Now train the model using the command 

* rasa train    

We can chat with the trained chatbot from the terminal itself, using the command 

* rasa shell 

Download ngrok and extract it from terminal and Then extract ngrok from the terminal

* sudo tar xvzf ~/Downloads/ngrok-v3-stable-linux-amd64.tgz -C /usr/local/bin

Start a tunnel using the command

* ngrok http 5005     

connect the Twilio WhatsApp API to a Rasa chatbot by set up a webhook that allows your chatbot to receive and respond to messages from the WhatsApp API

Now open two terminal,Enter into the virtual environment

Connected it to WhatsApp using twilioBy using the command in first terminal:

* rasa run -m models --enable-api --cors “*” –debug

and in the second terminal

* rasa run actions
