```
                     /$                               /$$   solanaizer/solanaizer-action
                    | $$                              |__/ 
  /$$$$$$$  /$$$$$$ | $$  /$$$$$$  /$$$$$$$   /$$$$$$  /$$ /$$$$$$$$  /$$$$$$   /$$$$$$
 /$$_____/ /$$__  $$| $$ |____  $$| $$__  $$ |____  $$| $$|____ /$$/ /$$__  $$ /$$__  $$
|  $$$$$$ | $$  \ $$| $$  /$$$$$$$| $$  \ $$  /$$$$$$$| $$   /$$$$/ | $$$$$$$$| $$  \__/
 \____  $$| $$  | $$| $$ /$$__  $$| $$  | $$ /$$__  $$| $$  /$$__/  | $$_____/| $$
 /$$$$$$$/|  $$$$$$/| $$|  $$$$$$$| $$  | $$|  $$$$$$$| $$ /$$$$$$$$|  $$$$$$$| $$
|_______/  \______/ |__/ \_______/|__/  |__/ \_______/|__/|________/ \_______/|__/
```

# Github Action for Solanaizer

This action enables you to run the Solana AI smart contract vulnerability scanning tool, Solanaizer, as part of your GitHub CI pipeline in the simplest possible way. There are many ways you can optimise the job, but this action aims to make things super easy!

## Running the Action in GitHub CI ♾️

You can use this Action as part of your project by creating an Action as follows:

```yaml
name: Solanaizer AI Audit

on:
  push:
    branches: main
  pull_request:
    branches: main

jobs:
  audit:
    runs-on: ubuntu-latest
    steps:
      - name: Check-out the repository
        uses: actions/checkout@v4
      - name: Solanaizer Audit
        continue-on-error: false
        uses: solanaizer/solanaizer-action
```

## Feedback 🤜🤛

Please raise an issue for suggestions and any bugs related to the Action.

## Responsibility 🤙

This is an experimental auditing tool built using AI. **USE AT YOUR RISK**

## Team 👨🏻‍💻👨🏻‍💻👨🏻‍💻👨🏻‍💻👨🏻‍💻

- [Alex Straw](https://github.com/alex-straw) (Engineer)
- [Dimitris Dinis Gridian](https://github.com/DinisDimitris) (Engineer)
- [Jean-Philippe Monette](https://github.com/jpmonette) (Engineer)
- [Michal Zbigniew Hoffman](https://github.com/MZHoffman) (Engineer)
- [Mikołaj Kącki](https://github.com/mkacki98) (Engineer)
