# Chainlink Keepers

Using Chainlink Keepers in a contract that increments a variable in each specified interval.

#### Requeriments to be a Keepers-compatible contract:

- Import KeeperCompatible.sol
- Use KeeperCompatibleInterface from the library
- Use checkUpkeep() bool function that says if performUpKeep() should be executed or not
- Use performUpkeep() function that will be executed when checkUpkeep() returns true
  it’s recommended to check the logic again within the performUpkeep(), to confirm that it should be called
