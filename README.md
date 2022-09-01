# Tools
This Repo contains quick tools, which can help in development faster.

# Docker commands 
# Jupiter notebook
docker run --rm -p 10000:8888 -e JUPYTER_ENABLE_LAB=yes -v "${PWD}":/home/jovyan/work jupyter/datascience-notebook:33add21fab64
# cloudbeaver
docker run --name cloudbeaver --rm -ti -p 7777:8978 -v /data/docker:/opt/cloudbeaver/workspace -d dbeaver/cloudbeaver:latest
# portainer 
docker run -d -p 9000:9000 -p 8000:8000 --name portainer --restart always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer
# How to reset git password ? 
git config --global --unset user.password
