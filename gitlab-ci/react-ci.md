# Configuration

Create a `.gitlab-ci.yml` file inside your project root directory and copy the below configuration.

```yaml
stages:
  - lint

lint:
  stage: lint
  image: node
  script:
    - echo "Code linting..."
    - npm install
    - npm run lint
```

> As of now we will only perform linting checks.