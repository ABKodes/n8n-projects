# Use the official n8n image as a base
FROM n8nio/n8n:latest

# Set environment variables for the container
ENV N8N_PORT=5678
ENV N8N_PROTOCOL=http
ENV NODE_ENV=production

# Expose the default n8n port
EXPOSE 5678

# Start n8n
CMD ["n8n", "start"]
