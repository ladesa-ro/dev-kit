compose_cname=ladesa-reverse-proxy
compose_options=--file docker-compose.yml -p $(compose_cname)

setup:
	$(shell (find . -type f -name "*.example" -exec sh -c 'cp -n {} $$(basename {} .example)' \;))
	$(shell (bash -c "docker network create $(d_network) &>/dev/null"))

up:
	make setup;
	docker-compose $(compose_options) up --force-recreate --remove-orphans -d;

logs:
	make setup;
	docker-compose $(compose_options) logs -f;

stop:
	make setup;
	docker compose $(compose_options) stop;

down:
	make setup;
	docker-compose $(compose_options) down --remove-orphans;

cleanup:
	docker compose $(compose_options) down --remove-orphans -v;