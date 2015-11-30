FROM tjake/jepsen 

RUN apt-get -y -q update 
RUN apt-get install -qqy unzip

RUN cd /jepsen && git config --global user.email "ryan.a.swanson@gmail.com" && git remote add zerbitx https://github.com/ZerbitX/jepsen && git remote update && git checkout -b consul-jepsen --track zerbitx/master && git pull zerbitx master
