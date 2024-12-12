# nextjs-test1

From NextJs Doc:
https://nextjs.org/docs/app/getting-started/installation

```
npx create-next-app@latest
```

From Prisma Doc:
https://www.prisma.io/docs/getting-started/quickstart-sqlite

```
npm install prisma --save-dev
npx prisma init --datasource-provider sqlite
```

Add models into `./prisma/schema.prisma` according to the doc:
```
npx prisma migrate dev --name init
```
Output:
```
Environment variables loaded from .env
Prisma schema loaded from prisma/schema.prisma
Datasource "db": SQLite database "dev.db" at "file:./dev.db"

Error: Schema engine exited. Error: Command failed with exit code 1: /mnt/sda3/nextJs/myapp-npm/node_modules/@prisma/engines/schema-engine-debian-openssl-3.0.x cli --datasource <REDACTED> can-connect-to-database
```

My Environment & setup
- OS: Linux Mint 22 Wilma based on Ubuntu 24.04 noble
- Database: using a plain TypeScript project and a local SQLite database file as described in the doc Quick Start page https://www.prisma.io/docs/getting-started/quickstart-sqlite
- Node.js version: v22.12.0
