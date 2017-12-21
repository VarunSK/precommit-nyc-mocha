nyc-mocha for pre-commit
========================

For pre-commit: see https://github.com/pre-commit/pre-commit

For nyc: see https://github.com/istanbuljs/nyc

### Using Prettier with pre-commit

Add this to your `.pre-commit-config.yaml`:
```yaml

    -   repo: https://github.com/VarunSK/precommit-nyc-mocha
        sha: ''  # Use the sha or tag you want to point at
        hooks:
        -   id: nyc-mocha
            args: [] #list of args like '--single-quote', '--jsx-bracket-same-line', '--print-width 120', '--no-bracket-spacing'
            additional_dependencies: ['nyc@11.4.1','mocha@4.0.1']
 ```   
