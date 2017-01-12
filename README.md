# rfcs

### Github doesn’t just mean source control, it’s a great community building tool.

Open source teams are naturally distributed by design, enterprise teams are looking to the open source community for ideas as to how to be better in this environment which is trending that way. Whether you're running an open source team or trying to get your enterprise teams to collaborate more an RFC process is a great way to get everyone involved.

Popular open source projects have the unenviable problem of communicating decisions and change, especially breaking changes, rust and ember are adopting an RFC process, this is something we have been trying for our team internally and it has worked great.

### Benefits to a github based RFC process

* Very low ceremony, easy to setup
* Uses the tools your developers already know and love
* Socialization of decisions encourages everyone to be involved
* Very useful if your team is distributed
* By doing written down avoids just the Type A personalities drowning out everyone else, <anecdote>
* Avoid watercooler conversations
* Build institutional knowledge, an archive of decisions and how the team got there
* Useful for new people to understand “context”
* Helps avoid the “new team rewrite” scenario
* Build a list of “team approved initiatives”
* New team members can find something the team had discussed, and regardless of level can find something to “own” day one, likely things the team wants to do but doesn’t have time to or hasn’t been a priority. 

### Challenges for enterprise teams

* Build institutional knowledge
* Try to avoid the “new team lets rewrite everything effect”

### How to create an RFC repo

1. Create a repo called RFCs (or clone this one)
1. Create a README and a markdown template
1. Define any labels you think are useful
1. Done!

### How to create an RFC

1. Create a new branch
1. Copy the template
1. Fill it out using markdown (vs code is excellent for this!)
1. Create a PR to start the conversation
1. Follow your usual workflow, maybe assign reviewers
1. When you have a way forward, merge the PR

### Leveling up?

1. Use projects to visualize RFC state?
1. Pages

### Dotcom vs. enterprise

Assigned review status, coming soon…
Pages

{% for decision in site.collections.decisions.docs %}
  <h2>{{ decision.title }}</h2>
{% endfor %}