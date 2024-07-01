# Speaking with a Webpage - Streaming Speech Transcripts || [GSP125](https://www.cloudskillsboost.google/course_templates/756/labs/475240) ||

# # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 👍😄🤝

* ### Run the following Commands in Cloudshell
```
export ZONE=
```
```
gcloud auth list

gcloud compute instances create speaking-with-a-webpage  --project=$DEVSHELL_PROJECT_ID --zone=$ZONE --machine-type=e2-medium --image=debian-11-bullseye-v20230509 --image-project=debian-cloud --scopes=https://www.googleapis.com/auth/cloud-platform --tags=http-server,https-server


sleep 15

gcloud compute ssh "speaking-with-a-webpage" --zone=$ZONE --project=$DEVSHELL_PROJECT_ID --quiet --command "sudo apt update && sudo apt install git -y && sudo apt-get install -y maven openjdk-11-jdk && git clone https://github.com/googlecodelabs/speaking-with-a-webpage.git && gcloud compute firewall-rules create dev-ports --allow=tcp:8443 --source-ranges=0.0.0.0/0 && cd ~/speaking-with-a-webpage/01-hello-https && mvn clean jetty:run" 
```
* ### Press CTRL+C to stop the server
* ## Check your progress on task 1-3 & Don't run the next command until you get the score
* ### Run the following Commands in Cloudshell
```
export ZONE=
```
```
gcloud compute ssh "speaking-with-a-webpage" --zone=$ZONE --project=$DEVSHELL_PROJECT_ID --quiet --command "pkill -f 'java.*jetty'"

sleep 10

gcloud compute ssh "speaking-with-a-webpage" --zone=$ZONE --project=$DEVSHELL_PROJECT_ID --quiet --command "cd ~/speaking-with-a-webpage/02-webaudio && mvn clean jetty:run"
```

# Congratulations ..!!🎉  You completed the lab shortly..😃💯

# *Well done..!* 👏

# Thank you for visiting.... :) 🗯️

# [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN)

