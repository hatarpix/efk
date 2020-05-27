# efk
EFK stack for docker swarm

1. Clone the repo https://github.com/hatarpix/efk.git
2. cd efk
3. Mark node for management logs
  - docker node ls
  - docker node update --label-add type=main {node_ID}
4. Deploy 

   docker stack deploy --compose-file docker-compose.yml efk
