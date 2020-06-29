+++
title = "Linux is the shit"
date = 2020-06-28
[taxonomies]
tags = ["programming, personal"]
+++

Well a lot has happened since the last post, from building another computer to trying to install some linux distros only to find out they don't support the new hardware yet. Mainly it's been gaming, I won't lie..but here's some programming at least.

# Linux

BSD and MacOS have these too, although they differ in the amount of prototypes they offer compared to the Linux kernel.

Syscalls learned:

- open()
- creat()
- read()
- write()

  Super neat to actually start using these in C, I've become obssesed over the idea of POSIX and SUS compliance. I'm actually more excited about learning the insides of Linux, but also not relying on the C std libs for everything. Even though these are just basic calls, they are the foundation of file access on linux and well worth learning; afterall we all must crawl before we can run. At some point I'll make another blog post detailing out these specific syscalls I learned, the code I wrote for each of them, and what I've learned about them. Although, there is one thing that I need to write down for the sake of it. The read() call is very interesting, it allows you to think of files as more than just something that might hold a textual value. This is because in linux, everything is essentially accessed like a file. Everything from devices to pipes, sockets, etc. This is a very interesting concept, because unlike most read accesses from a text file (which get read to EOF), read can also read from a network socket and block (sleep) while it waits for data to pass through the socket and into the file descriptor (fd). On the flip side, this also means that the read might also return partially read, if the connection interrupts. This teaches us to do quite a lot of error checking, which will allow for more efficient code. Super neat stuff.

  # Rant

  Detailing a little bit futher on the first paragraph, I've gone through several different ideas. From gaming to distro hopping, I've be having a hard time (as I always seem to these days) with sticking to one particular task. I'm like the friend you know who shows up with a different car every day and for no real reason. I just do it because my mind jumps from idea to idea, when I'm studying something for a moment then my mind gets distracted and thinks of something else to do. Sometimes it's bordem, like when I watch lectures, and just want to skip to actually doing something instead of observing for hours at a time. The main time sinker is the IDEA of doing something, but then actually doing it turns out to be a waste of time. With this in mind, I need to be more conditioned to weighing out the positives vs the negatives of doing a task so that I might not regret it in the future. I always thought that maybe I'm just not that bright or have a hard time understanding, and part of that is true. I do believe I have some type of learning disability, especially when it comes to retaining information or even just reading a book and recalling what I read. However, I do spit out code in the end and I suppose I do learn something, it's just that it takes a monumental effort to do so, but perhaps others have this problem too. I feel like it shouldn't be so hard to learn, especially if I have a background in a similar area of interest.
