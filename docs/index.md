<i>Some musings about stuff I find interesting</i>

---

### Rob Pike's 5 rules of programming.

November 1, 2023

I first started following Rob Pike from when he worked on GoLang. He obviously has a lot of prior experience, but that was when I first came to know of him. His works always were so insightful && his five rules for programming ring so true, that they are worth repeating ad infinitum. 


1. You can't tell where a program is going to spend most of its time. Bottlenecks occur in surprising places, so don't try to second guess and put in a speed hack until you've proven that's where the bottleneck is.

2. Measure. Don't tune for speed until you've measured, and even then don't unless one part of the code overwhelms the rest.

3. Fancy algorithms are slow when n is small && n is usually small. Fancy algorithms have big constants. Until you know that n is frequently going to be big, don't get fancy. (Even if n does not get big, use Rule 2 first)

4. Fancier algorithms are buggier than simpler ones, and they're much harder to implement. Use simple algorithms as well as simple data structures.

5. Data dominates. If you've chosen the right data structures and organized things well, the algorithms will almost always be self evident. Data structures, not algorithms, are central to programming.

Source: [https://users.ece.utexas.edu/~adnan/pike.html](https://users.ece.utexas.edu/~adnan/pike.html)
