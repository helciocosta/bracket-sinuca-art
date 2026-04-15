# Development image
FROM node:25-alpine

WORKDIR /app

# Install pnpm
RUN apk add --no-cache pnpm

# Copy package files
COPY package.json pnpm-lock.yaml* ./

# Install dependencies
RUN pnpm install

# Copy source
COPY . .

# Expose Vite dev port
EXPOSE 5173

# Run Vite in dev mode with host binding
CMD ["pnpm", "dev", "--host", "0.0.0.0"]
