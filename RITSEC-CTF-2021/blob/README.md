# Problem : blob

'' Ha. Blob. Did you get the reference?

http://git.ritsec.club:7000/blob.git/ ''

## Analysis

So from the Problem Description it was clear that the git repo had the flag in one of it's blobs.
So I used the command I found on StackOverflow [here](https://stackoverflow.com/questions/1595631/how-to-get-a-list-of-all-blobs-in-a-repository-in-git "here") : 
>$ git rev-list --objects --all | git cat-file --batch-check='%(objectname) %(objecttype) %(rest)' | grep '^[^ ]* blob' | cut -d" " -f1,3-

It returned :
>d0644363aa853a17c9672cefff587580a43cf45e
>e597cc86a0881ab3028dba090f88c1cbd33ad9a4 README.md
>df576e13e1ca1c4310d3260f63bef4db41218ba0 flag.txt

The flag.txt was useless and only had "these aren't the droids you're looking for" written inside it.

So the only information remains to the standalone blob which I read with :
> $ git cat-file -p d0644363aa853a17c9672cefff587580a43cf45e

And it returned the flag:
> RS{refs_can_b3_secret_too}