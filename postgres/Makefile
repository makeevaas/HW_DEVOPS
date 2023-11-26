DOCKER_IMAGE_NAME := "postgres"
VERSION := latest

.PHONY: postgres
postgres:
	@docker run -it --rm \
		--name pg-container \
		--env POSTGRES_USER=test \
		--env POSTGRES_PASSWORD=test \
		--env POSTGRES_DB=test \
		-p 5432:5432 \
    postgres:latest

.PHONY: postgres-cli
postgres-cli:
	@docker exec -it pg-container psql -U test