# BasicSVN
A very basic svn client which supports pseudo-local commits, and is free and open source (woo!).

---

# Planned features
- View change list
- Integrated diff
- Option to open external diff tool (a better one...)
- Standard svn commands
- Pretend local commits

# What do you mean by "pseudo-local" ?
As you probably know, SVN doesn't allow for local commits. This is very annoying.
My plan is to allow copying current changes into a separate location, with a commit message.
Then these pretend local commits can be sent off as real commits by automatically rolling back
the real working copy to the state it was in when that local commit was made, then undoing those
changes.

I'm sure whatever I end up with will be a little bit janky, but honestly it should be easier
than using git-svn for simple cases. 
...all I want is to break up monolothic commits damn it. I don't actually need the full might of git.