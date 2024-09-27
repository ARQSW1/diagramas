FROM plantuml/plantuml

RUN apt-get update \
  && apt-get install --no-install-recommends -y \
    git-all \
  && apt-get autoremove \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*


ENTRYPOINT ["java", "-jar", "/opt/plantuml.jar"]
CMD ["-version"]