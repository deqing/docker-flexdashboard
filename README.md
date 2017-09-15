# docker-flexdashboard

Docker container for [flexdashboard - Easy interactive dashboards for R][1]

## Install dependencies

  - [Docker][2]

To install docker in Ubuntu 14.04 use the commands:

    $ sudo apt-get update
    $ wget -qO- https://get.docker.com/ | sh

To install docker in other operating systems check [docker online documentation][3]

## Build Docker container

To build container use the command below:

    $ cd ~/docker-flexdashboard/
    $ docker build -t flexdashboard:latest .

## Run Docker container

To run container try the command below:

    $ docker run --rm -d -p 3838:3838 -v /home/yourname/flexdashboard/:/srv/shiny-server/ -v /home/yourname/flexdashboard/log/:/var/log/shiny-server/ flexdashboard

## Accessing your deployed applications:

Check with your browser at addresses plus the port 3838 :

  - **http://host_ip:3838/**

[1]:http://rmarkdown.rstudio.com/flexdashboard/
[2]:https://www.docker.com
[3]:http://docs.docker.com
