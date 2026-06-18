# SBA 302 - Version Control Reflection

## Branch Management
For this project, I created two feature branches to simulate a team development workflow. 
I created `feature/header` to add the header section of the webpage, committing the initial 
HTML structure with a navigation bar. I then created `feature/footer` to add the footer 
section independently, which mirrors how developers on a team would work on separate features 
simultaneously without interfering with each other's code.

## Handling the Merge Conflict
A merge conflict was deliberately triggered by modifying the footer section on both `main` 
and `feature/footer` with different content. When I attempted to merge `feature/footer` into 
`main`, Git could not automatically resolve the difference between the two footer lines and 
halted the merge. Git flagged the conflict in `index.html` using conflict markers to show 
the current change versus the incoming change. I resolved the conflict manually by reviewing 
both versions and accepting both lines of content, keeping the SecureGov company copyright 
line and the David Edwards copyright line. After resolving the file, I staged it with 
`git add` and committed the resolution with a descriptive message. This process taught me 
that conflicts are not errors — they are Git asking for a human decision when it cannot 
determine which change takes priority.

## Pull Request Process
After pushing all changes to GitHub, I created a pull request from `main` into `review/main`. 
The PR provided a clear visual diff showing exactly what changed between the two branches, 
including the commit history and the specific lines added. In a real team environment, this 
is where a senior developer or peer would review the code before it gets merged into 
production. The PR process creates a checkpoint that enforces code quality, catches mistakes, 
and documents why changes were made. It also provides an audit trail of decisions made 
during development.
