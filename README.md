**Deploy policies and workflows to maintain application security at the scale of a repository.**

The policy takes part in awareness by communicating useful information:
- [.github/SECURITY.md](.github/SECURITY.md)
  - communicate application security policy
  
The workflow automates the maintenance of application security:
- [.github/workflows/dependabot.yml](.github/workflows/dependabot.yml)
  - maintain open-source dependencies with **Dependabot** (https://github.com/dependabot)
- [.github/workflows/nuclei.yml](.github/workflows/nuclei.yml)
  - maintain dynamic application security testing with **Nuclei** (https://github.com/projectdiscovery/nuclei)
- [.github/workflows/codeql.yml](.github/workflows/codeql.yml)
  - maintain static application security testing with **CodeQL** (https://github.com/github/codeql)

The DAST and SAST workflows send data to Slack and DataDog for further investigation.
