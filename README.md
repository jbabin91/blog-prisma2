# Fullstack Blog Application with Prisma 2, Next.js, and Docker

## Getting Started

Download the project

```sh
git clone https://github.com/jbabin91/blog-prisma2
```

1. Rename `.env.example` to `.env`

2. Run `npm run build` in the root directory.

3. Run `npm start` in the root directory.

4. If you are running this for the first time after a build, you need to migrate the database. Run `npm run migrate`. Then run `npm stop` followed by `npm start` to reset the server.

## GraphQL API Info

### Queries

- Read all published blog posts
- Read all draft blog posts
- Read all users

### Mutations

- Create a user
- Create a blog draft
- Publish a blog
- Delete a blog

## Helpful commands

In the root directory:

`npm run build` This will build your frontend, backend, and prisma docker containers

`npm start` This will start up your docker compose docker containers

`npm stop` This will brin down the cluster and remove containers

`npm run clean` This will delete all containers, images, docker networks, etc...

`npm run clean:volumes` This will delete all docker volumes

`npm run generate` This will build `frontend/generated/apollo-components.tsx` based on the queries and mutations in the `frontend/graphql` folder that it will run against the backend server itself.
