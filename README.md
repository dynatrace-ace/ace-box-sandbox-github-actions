# ace-box-sandbox-github-actions

This ACE-BOX external use case is an example of how you can integrate Github actions and Sonarqube.

## Components deployed

The following components get deployed:

- microk8s
- Dynatrace Operator with OneAgent and Kubernetes ActiveGates
- Dynatrace CloudAutomation (Keptn)
- Dynatrace Monaco CLI
- Sonarqube
- Monitoring as Code configuration is applied
- Dashboard with predefined links

## Running the sandbox

Check out [ace-box documentation](https://github.com/Dynatrace/ace-box/blob/dev/docs/external-use-case.md) for more information and provite this git repo URL as the use-case!

```
use_case="https://github.com/dynatrace-ace/ace-box-sandbox-github-actions.git"
```

In addition, the following extra vars need to be provided:
```
extra_vars = {
  github_user        = "" # Github user name that has permissions to create repos in specified organization
  github_token       = "" # Github password
  github_org         = "" # Github organisation repositories will be created in
  github_repo_prefix = "" # string all repositories will be prefixed with
}
```

## References

- https://github.com/SonarSource/helm-chart-sonarqube
