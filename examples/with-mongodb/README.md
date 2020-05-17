# MongoDB and Next.js Example 

This example shows how you can use MongoDB as database to support your Next.js application

## Demo 

### Pets: https://with-mongodb-navy.now.sh/

**Pets** - an application that allows users to add their pets' information (e.g., name, owner's name, diet, age, dislikes, likes, and photo). They can also delete it or edit it anytime.

## How to use

### Using `create-next-app`

Execute [`create-next-app`](https://github.com/zeit/next.js/tree/canary/packages/with-mongodb-app) with [npm](https://docs.npmjs.com/cli/init) or [Yarn](https://yarnpkg.com/lang/en/docs/cli/create/) to bootstrap the example:

```bash
npm init next-app --example with-mongodb with-mongodb-app
# or
yarn create next-app --example with-mongodb with-mongodb-app
```

### Configuration

#### Step 1. Connect MongoDB to the application

Please see the [steps](./link-step.md) on how to connect MongoDB to your application

#### Step 2. Set up schema models for the application

Based on the types of data needed for your application, you will modify the type definitions in [Pet.js](./models/Pet.js) as well as the seed data in [Pet-sampleSeed.json](./seed/Pet-sampleSeed.json)

#### Step 3. Import sample seed data to your MongoDB

Please see the [steps](./data_import.md) on importing sample seed data into your MongoDB

#### Step 4. Change ROOT_URL

Set ROOT_URL in [next.config.js](./next.config.js) to ```http://localhost:3000```

### Install it and run:

```bash
npm install
npm run dev
# or
yarn
yarn dev
```
### Deploy

Set the production URL given by ZEIT Now as the ROOT_URL in the next.config.js file. The add, delete, and edit functionality will only work in the production link.

Deploy it to the cloud with [ZEIT Now](https://zeit.co/import?filter=next.js&utm_source=github&utm_medium=readme&utm_campaign=next-example) ([Documentation](https://nextjs.org/docs/deployment)).

© 2020 GitHub, Inc.
