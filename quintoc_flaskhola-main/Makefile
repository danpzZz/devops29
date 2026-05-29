deployconip:
|	@ docker run -d --name appflask -p 7000:5000 ghcr.io/danpzzz/appflask:2.0

deploy:
	@ docker stack deploy  -- with-registry-auth -c stack.yml daniel

network:
	@ docker network create --driver overlay --scope swarn daniel_net || true

volume:
	@ docker volume create v_daniel