1-Install Docker 

2-command build docker image 

docker build -t  userid/repositoryname .


3-Install npm (remove node_module in your project then install)

 docker run -ti --rm   -p 8100:8100  -v ${PWD}:/myApp:rw userid/repositoryname npm install


4-command serve ionic project in localhost 

docker run -ti --rm   -p 8100:8100  -v ${PWD}:/myApp:rw userid/repositoryname ionic serve --port 8100 --address=0.0.0.0


5-command build android apk

 docker run -ti --rm   -p 8100:8100  -v ${PWD}:/myApp:rw userid/repositoryname ionic cordova build android



