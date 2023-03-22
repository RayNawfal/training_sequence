# training_sequence
Chatbot training model in the form of a Scramjet Sequence

For installing packaging dependencies required from requirements.txt <br/>
`pip3 install -t __pypackages__ -r requirements.txt`

Pack a sequence into a tar.gz file.<br/>
`si seq pack <path/to/folder>`

Start STH with:<br/>
`DEVELOPMENT=true yarn start  --runtime-adapter=docker`<br/>
`si seq send training_sequence.tar.gz --progress`<br/>
`si seq start <seq-id>`<br/>

`$ docker ps` <br/>

|CONTAINER ID__|IMAGE_________________________|         COMMAND___________|         CREATED_______|    STATUS________|PORTS_________|   NAMES  <br/>
|__\<container-id>____|__scramjetorg/runner-py:0.33.1 |  "/usr/bin/tini -- do…" |  4 seconds ago___| Up 2 seconds_______|________________|  youthful_davinci

`docker exec -ti <container-id> /bin/bash`  <br/>

#Inside container <br/>
`python -m pip install numpy`
