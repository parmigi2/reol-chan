# Notice

reol-chan has undergone a rewrite! https://github.com/causztic/reol-chan/releases/tag/1.0.0

Legacy code is in the `senpai` branch.

## Setup
- Install [Node.js](https://nodejs.org/en/download/current)
- Install [PostgreSQL](https://www.postgresql.org/download/) and create a database
- Create a discord application on [Discord developers portal](https://discord.com/developers/home)
- Rename `.env.example` into `.env` and update it with your values
- Install requirements
```
npm install
```
- Load the database's schema
```
npx prisma migrate deploy --config prisma/prisma.config.ts
```
- Start
```
npm start
```

Run `prisma studio --config prisma/prisma.config.ts` to visualise the database's data

Run `prisma generate` on schema changes

## Roadmap

- [x] Typescript
- [x] ESLint
- [x] Slash command integration with Discord.js 14
- [x] Role Management port-over
- [x] Now playing port-over
- [ ] Points port-over (Redis)
- [ ] Postgres port-over (migrations not necessary yet)
- [ ] Discography Management port-over

## Non-essential Roadmap

- [ ] S3 library port-over
- [ ] Purge port-over
- [ ] CI/CD
