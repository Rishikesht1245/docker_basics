FROM kasmweb/ubuntu-focal-desktop:1.15.0

USER root
# Install Node.js
RUN curl -fsSL https://deb.nodesource.com/setup_22.x | bash - && \
    apt-get install -y nodejs && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Optional: Verify Node.js and npm installation
RUN node -v && npm -v

# Set the default user to root
USER root

# Entry point
CMD ["start-kasm"]