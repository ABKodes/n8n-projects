# Use the official n8n image as a base
FROM n8nio/n8n:latest

# Set environment variables
ENV N8N_PORT=5678
ENV N8N_PROTOCOL=http
ENV NODE_ENV=production

# You can add custom node installations here if needed
# RUN npm install -g n8n-nodes-custom-example

# We don't copy the workflow JSON directly into the image to keep it flexible.
# Instead, it's recommended to mount it via docker-compose or import it.

EXPOSE 5678

CMD ["n8n", "start"]
