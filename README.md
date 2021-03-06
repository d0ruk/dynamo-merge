# dynamo-merge

[![Greenkeeper badge](https://badges.greenkeeper.io/wolverian/dynamo-merge.svg)](https://greenkeeper.io/)
[![Build Status](https://travis-ci.org/wolverian/dynamo-merge.svg?branch=master)](https://travis-ci.org/wolverian/dynamo-merge)
[![NPM Version](https://img.shields.io/npm/v/dynamo-merge.svg)](https://www.npmjs.com/package/dynamo-merge)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/d8132eb0d9a94e7bb6a349ffa291dc66)](https://www.codacy.com/app/ilmari.vacklin/dynamo-merge?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=wolverian/dynamo-merge&amp;utm_campaign=Badge_Grade)

## Installation

```shell
yarn add dynamo-merge # or npm install dynamo-merge --save
```

## Usage

``` js
import merge from "dynamo-merge"

const result = await documentClient.update({
    TableName: "users",
    Key: {email},
    ...merge(updatedUserAttributes),
})
```

Look at `test.js` for example use cases and the expected output.

## Tests

To run tests, use

``` shell
yarn test # or npm test
```

## License

MIT
