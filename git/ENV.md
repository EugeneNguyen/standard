# CD/CI branch strategy

## Env recommended

| Env         | Purpose                                                       |
|-------------|---------------------------------------------------------------|
| Development | For internal testing                                          |
| Staging     | For customer testing                                          |
| Beta        | For customer testing in real database, maybe for beta testing |
| Production  | Real code, real database. No testing here                     |

## Git branch strategy integrated with Environment

### Environment and Branch / Database

| Env         | Branch                    | Database         |
|-------------|---------------------------|------------------|
| Development | develop                   | Testing database |
| Staging     | release                   | Staging database |
| Beta        | master - automatic deploy | Real database    |
| Production  | master - manual deploy    | Real database    |
