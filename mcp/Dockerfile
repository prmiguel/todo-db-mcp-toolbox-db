FROM us-central1-docker.pkg.dev/database-toolbox/toolbox/toolbox:latest

COPY  tools.yaml /config/tools.yaml
EXPOSE 5000

CMD ["toolbox", "--tools-file", "/config/tools.yaml", "--address", "0.0.0.0"]
