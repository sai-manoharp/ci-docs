# Configuration

Create a `.gitlab-ci.yml` file inside your project root directory and copy the below configuration.

```yaml
stages:
  - lint  

lint:
  stage: lint
  script: 
    - echo "Linting code..."
    - composer install
    - composer run lint
    - echo "Static code analysis..."
    - composer run phan
```

> As of now we are performing linting and static analysis. 

