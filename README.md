# MPCS 53001 - Assignment 4

### Spencer Dearman

## Setup

1. Run `npm install` in the root directory. Note, if you get a chalk error (I did
   once so just in case) run `npm uninstall chalk` then `npm install chalk@4`

2. **Setup assumes that you have the sakila MySQL dabatase locally (localhost)**.
   Go to the [data-sources.ts](src/data-sources.ts) file and edit **line 12** to add your
   own root password.

## Commands

#### Init Command

`npx ts-node src/index.ts init`

#### Full-Load Command

`npx ts-node src/index.ts full-load`

#### Incremental Command

`npx ts-node src/index.ts incremental`

#### Validate Command

`npx ts-node src/index.ts validate`

#### Delete Database

`rm analytics.db`

## Tests

#### Run All Tests

`npm test`

#### Run Init Test

`npm test -- -t "Init"`

#### Run Full-Load Test

`npm test -- -t "Full-load"`

#### Run Incremental (new data) Test

`npm test -- -t "3. Incremental command"`

#### Run Incremental (no new data) Test

`npm test -- -t "4. Incremental command"`

#### Run Validate Test

`npm test -- -t "Validate"`
