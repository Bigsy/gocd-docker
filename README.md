# go.cd based CI installation

docker build -t ovo/gocd-agent -f Dockerfile.bosp-gocdagent .

docker run -t -i --privileged -d -e GO_SERVER=XXXXX-e GO_SERVER_PORT=8154 --name gocd-agent ovo/gocd-agent

