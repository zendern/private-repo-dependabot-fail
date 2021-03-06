# private repo dependabot fail 

2 projects live here. One gradle and another maven.

Both have been configured to never talk to maven central or any other private repos. 

In the gradle case, dependabot will no open PRs b/c the private repo can never be resolved. 

In the maven case, (looking at the code and hopefull new prs soon) it automatically will add
maven central to the list of repos so that it can resolve even though the project only allows
private repos. 