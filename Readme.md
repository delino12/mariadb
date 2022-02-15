## Read Me

Run the command below on your terminal

docker network ls | grep yournetworkname > /dev/null || docker network create \
  --ipam-driver=default --gateway=172.30.0.1 --attachable=true \
  --driver=bridge --subnet=172.30.0.0/16 yournetworkname


Remember to update `yournetworkname` with the exact network name you'd love to use. 
