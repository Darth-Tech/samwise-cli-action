# samwise-cli-action
GitHub action to check your outdated custom Tf modules and update the report to the pull request. Uses [samwise-cli]() under the hood.


## Usage
```yaml
	- name: samwise-tf-modules-update-report
	  uses: Darth-Tech/samwise-cli-action@v0.1.13
	  with:
		  SAMWISE_CLI_GIT_USER: gdna-devops
		  SAMWISE_CLI_GIT_KEY: ${{ secrets.GIT_ACCESS_TOKEN }}
		  GIT_ACCESS_TOKEN: ${{ secrets.GIT_ACCESS_TOKEN }}
		  DEPTH: 0
		  REPO_PATH: .
		  IGNORE: ".git,.github,.idea"
		  VERBOSITY: info
```
