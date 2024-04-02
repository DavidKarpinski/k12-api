# local_api
API required for Blog K-12 project

## Installation

```bash
git clone https://github.com/DavidKarpinski/local_api.git

npm i
# or
yarn

json-server --watch db.json # Must run on port 3000
```

By default, JSON Server runs on https://localhost:3000.

In case of an error like: `Some error occurred Error: listen EADDRINUSE: address already in use ::1:3000`, 
This is because some project is already running on port 3000 and to do so, simply add a different number such as `-p=<portnumber>` as shown in the example:

```
json-server --watch db.json -p=3001
```

It is worth mentioning that any port change in the API will require adaptations to the code of the programs that use it.
