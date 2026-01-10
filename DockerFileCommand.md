# Set base image
FROM <image>

# Execute command during build
RUN <command>

# Default command when container starts
CMD ["executable", "param"]

# Configure container as executable
ENTRYPOINT ["executable"]

# Copy files from host to image
COPY <src> <dest>

# Copy files (supports URLs and tar)
ADD <src> <dest>

# Set working directory
WORKDIR /path

# Set environment variable
ENV KEY=value

# Document exposed ports
EXPOSE <port>

# Create mount point
VOLUME ["/data"]

# Set user for RUN, CMD, ENTRYPOINT
USER <username>

# Add metadata to image
LABEL key=value

# Build-time variables
ARG <name>=<default>

# Health check
HEALTHCHECK CMD <command>

# Set shell for RUN commands
SHELL ["executable", "parameters"]


# Add trigger instruction
ONBUILD <instruction>

# Set stop signal
STOPSIGNAL <signal>
