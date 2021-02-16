# Commit Message Guidelines
Here's a nifty template to follow:

```bash
<type>(<lang>): <subject>       # <lang> is optional

<body>

<footer>
```

## Example commit:
```bash
fix(middleware): ensure Range headers adhere more closely to RFC 2616

Add one new dependency, use `range-parser` (Express dependency) to compute
range. It is more well-tested in the wild.

Fixes #2310
```


## Summary, or the git subject line
After listing the commit `<type>` (and potential scope/lang), write what changes will be applied, (i.e. `fix: correct typos in jasper-notes.md`)

### Allowed `<type>` values
| value[^1]    | description                                       |
| -------- | ------------------------------------------------- |
| chore    | cleaning up code; no changes to production code   |
| docs     | documentation edits and changes                   |
| feat     | new user features (not for build-script features) |
| fix      | bug fixes \>\_\<                                  |
| refactor | tasks like renaming variables in src code         |
| style    | fix formatting issues like missing semi-colons    |
| test     | adding tests                                      | 


##  Message body 
Here is where to write your motivation for the changes, highlight contrasts with prior behavior. Use the message body to explain what and why you have done something.

- **The first line of a commit is the most important line of that commit.**
This line is \*special\*. We don't have to worry about what makes it so special, but just keep in mind that this first line needs to be a a) summary of the change itself and b) mentions any part of the code affected by this change. Maybe this seems silly, but it's useful for when you're working with others!

Whatever you write here should be self-contained, i.e. reading the commit doesn't require any external references to fully understand what you're talking about.

### The following is a list of questions you should aim to answer in a commit message:
- What (original) problem is addressed by this commit?
- How is this problem being fixed? What changes did you make to fix it?
    - also good practice: describe the intent of the fix applied and possibly the motivation behind said fixes.
- Why is a change being made, or, what is the original problem?
- What change did you make? 
    - provide detailed description
    - write as many paragraphs as you'd like, or a few as you want, just try to give enough info that any can easily understand what you did
- What limitations still exist in the code?
    - Helpful for roadmapping 

I know remembering all that is not easy for us, the world's most forgetful humans, so at the very least try to keep this key idea in mind:

<pre style="padding:10px;margin:0 0 10px;background:#eee;color:#F5319D;font:14px/1.5 monospace;">The commit message must contain all the information required to fully understand &amp; review the patch for correctness. <i>Less is <b>not</b> more. More is more.</i>
</pre>
    
### (3) Footer 
In the footer you should reference the issues this commit addresses or closes (see example below). 

Any breaking changes should be mentioned here as well.[^0]


- Bullet points are okay, too.
- Typically a hyphen or asterisk is used for the bullet, followed by a
  single space. Use a hanging indent.



Details for each point and good commit message examples can be found on https://wiki.openstack.org/wiki/GitCommitMessages#Information_in_commit_messages

### References in commit messages
If the commit refers to an issue, add this information to the commit message header or body. e.g. the GitHub web platform automatically converts issue ids (e.g. #123) to links referring to the related issue. For issues tracker like Jira there are plugins which also converts Jira tickets, e.g. [Jirafy](https://chrome.google.com/webstore/detail/jirafy/npldkpkhkmpnfhpmeoahhakbgcldplbj).

In header:
```
[#123] Refer to GitHub issue…
```
```
CAT-123 Refer to Jira ticket with project identifier CAT…
```
In body:
```
…
Fixes #123, #124
```

### Sources
* http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html
* https://wiki.openstack.org/wiki/GitCommitMessages
* http://chris.beams.io/posts/git-commit/





[^1]: don't worry, we'll add, edit, and cull these as we figure out what works best for us
