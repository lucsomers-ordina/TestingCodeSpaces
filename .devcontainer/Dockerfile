FROM ampersandtarski/ampersand:v4.7

COPY --from=ampersandtarski/ampersand:v4.7 /bin/ampersand /usr/local/bin
RUN chmod +x /usr/local/bin/ampersand

# Set `DEVCONTAINER` environment variable to help with orientation
ENV DEVCONTAINER=true

RUN echo "\n\nif [ -d ~/.bashrc.d ]; then\n  for rc in ~/.bashrc.d/*rc; do\n    . \$rc\n  done\nfi\n" >> usr/local/bin/.bashrc