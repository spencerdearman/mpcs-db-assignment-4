# MPCS 53001 - Assignment 4
### Spencer Dearman

## Setup
1. Run `npm install` in the root directory. Note, if you get a chalk error (I did
once so just in case) run `npm uninstall chalk` then `npm install chalk@4`


# Delete the old file
rm analytics.db

# Re-create the empty tables
npx ts-node src/index.ts init

# Run the new load
npx ts-node src/index.ts full-load