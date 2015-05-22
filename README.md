### Commet description ###

Comparing and combining multiple metagenomic datasets

### Import the dockerfile ###

git clone https://github.com/cmonjeau/docker-commet.git

### Build the dockerfile ###

docker build -t cmonjeau/commet .

### Print commet help ###

docker run -it --rm cmonjeau/commet

### Run commet with data (inside /home/user/commet directory)

docker -H 127.0.0.1:2375 run -it --rm -v /root/Commet:/data cmonjeau/commet /data/sets_config.txt -k 33 -o /data/results

