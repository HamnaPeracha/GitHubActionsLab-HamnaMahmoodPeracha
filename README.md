# GitHubActionsLab-HamnaMahmoodPeracha


# Workflow 1: Dependent Jobs Workflow

# Purpose
This workflow demonstrates job dependencies by using a keyword `needs`.  
The jobs run in a specific order:
build → test → deploy.

# Key Concepts Demonstrated
`needs` keyword for job dependencies
`runs-on` to specify runner environment
Sequential job execution
Workflow triggered on push to main branch



# Workflow 2: Multi-Platform Workflow

# Purpose
This workflow demonstrates running jobs in parallel on multiple operating systems using different runners.

The jobs run on:
ubuntu-latest
windows-latest
macos-latest

# Key Concepts Demonstrated
`runs-on` with different operating systems
Parallel job execution
Workflow triggered on pull_request
Environment variables and runner differences



# Challenges Faced

1. Windows command syntax difference (`mkdir -p` not working).
   - Resolved by using Windows-compatible commands.

2. Understanding how pull_request triggers work.
   - Resolved by creating a new branch and opening a pull request.

3. Ensuring jobs ran in correct order.
   - Used the `needs` keyword properly.



# Conclusion

This lab demonstrated how GitHub Actions workflows can:
Run sequential jobs using dependencies
Run jobs in parallel on different operating systems
Automatically trigger workflows on push and pull request events