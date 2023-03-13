# Nextjs13 With Docker - Multiple Deployment Environments (Customised)

This examples shows how to use Docker with Next.js and deploy to multiple environment with different env values. Based on the [deployment documentation](https://nextjs.org/docs/deployment#docker-image).

# How to use
## Using Docker and Makefile

Make sure Docker is installed. If not, [download here](https://docs.docker.com/get-docker/)

### Development environment - for doing testing

```
make build-development
make start-development
```

Open http://localhost:3001

### Staging environment - for doing UAT testing

```
make build-staging
make start-staging
```

Open http://localhost:3002

### Production environment - for users

```
make build-production
make start-production
```

Open http://localhost:3003

## Running Locally

First, run the development server:

```bash
pnpm run dev
```

If you don't have pnpm installed, follow instructions [here](https://pnpm.io/installation)

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.