## Get a *free* weekly practice problem!

Keep that axe sharp.

<span class="input-group-btn"> </span>

No spam, ever. Easy unsubscribe.

*Cool, watch your inbox!*

<span class="small">[× No thanks]()</span>

<span class="navbar-brand"> <img src="/static//images/cake_white_20_21.png" class="logo" /> Interview Cake </span>

<span class="sr-only">Toggle navigation</span> <span class="icon-bar"></span> <span class="icon-bar"></span> <span class="icon-bar"></span>

<a href="/" class="navbar-brand">Interview Cake</a>

-   <a href="" class="dropdown-toggle">Interview Tips <span class="caret"></span></a>
    -   [First coding interview? Start here.](/coding-interview-beginner-faq)
    -   [General coding interview tips](/coding-interview-tips)
    -   [How to get un-stuck](/tricks-for-getting-unstuck-programming-interview)
    -   [Beating impostor syndrome](/impostor-syndrome-in-programming-interviews)
    -   [24 hours before your onsite](/24-hours-before-onsite-whiteboard-coding-interview)
    -   [Why you're hitting dead ends](/why-youre-hitting-dead-ends-in-whiteboard-interviews)
    -   [Best ways to practice](/getting-the-most-from-coding-interview-practice-sessions)
    -   [Organizing your interview timeline](/coding-interview-timeline-exploding-offers-burnout-negotiation-leverage)
    -   [Mastering behavioral questions](/behavioral-questions-programming-interview-story-telling)
    -   [Common issues](/coding-interview-faq)
-   <a href="" class="dropdown-toggle">Glossary <span class="caret"></span></a>
    -   [Big O Notation: <span complexity="n"></span>, <span complexity="n^2"></span>, etc](/big-o-notation-time-and-space-complexity)
    -   [Logarithms](/article/logarithms)
    -   [Triangular Series](/concept/triangular-series)
    -   
    -   [Binary Search](/concept/binary-search)
    -   [Breadth-First Search](/concept/bfs)
    -   [Depth-First Search](/concept/dfs)
    -   
    -   [Brute Force Algorithms](/concept/brute-force)
    -   [Greedy Algorithms](/concept/greedy)
    -   [Bottom-Up Algorithms](/concept/bottom-up)
    -   [Overlapping Subproblems](/concept/overlapping-subproblems)
    -   [Memoization](/concept/memoization)
    -   
    -   [Short Circuit Evaluation](/concept/short-circuit-evaluation)
    -   [Garbage Collection](/concept/garbage-collection)
    -   [Closure](/concept/js-closure)
    -   [Array Slicing](/concept/slice)
    -   [Hashing](/concept/hashing)
    -   [Mutable vs Immutable](/concept/mutable)
    -   [In-Place Operation](/concept/in-place)
    -   
    -   [Data Structures Overview](/article/data-structures-computer-science)
    -   [Array](/concept/array)
    -   [Dynamic Array](/concept/dynamic-array)
    -   [Hash Table](/concept/hash-map)
    -   [Linked List](/concept/linked-list)
    -   [Queue](/concept/queue)
    -   [Stack](/concept/stack)
    -   [Binary Tree](/concept/binary-tree)
    -   [Graph](/concept/graph)
    -   
    -   [Binary Numbers](/concept/binary-numbers)
    -   [Bitwise AND](/concept/and)
    -   [Bitwise OR](/concept/or)
    -   [Bitwise XOR](/concept/xor)
    -   [Bitwise NOT](/concept/not)
    -   [Bit Shifting](/concept/bit-shift)
    -   [Integer Overflow](/concept/integer-overflow)
-   [Full Course](/table-of-contents)

<!-- -->

-   <a href="/upgrade" class="upgrade">Get the full course <span class="glyphicon glyphicon-chevron-right full-access-badge"></span></a>

-   <a href="" class="dropdown-toggle"><span data-ng-bind="contentLanguage.display_name"></span> <span class="caret"></span></a>
    -   []()

-   <span class="glyphicon glyphicon-star full-access-badge" ng-show="currentUser.is_full_access"></span>

-   [Log out]()

-   [Log in to save progress]()

[<span class="glyphicon glyphicon-arrow-left"></span> The Intuitive Guide to Data Structures and Algorithms](/data-structures-and-algorithms-guide)

# <span style="display:inline-block;"> Data Structures for </span> <span style="display:inline-block;"> Coding Interviews </span>

## Computer science in plain English

To really understand how data structures *work*, we're going to derive each of them from scratch. Starting with bits.

Don't worry—we'll skip the convoluted academic jargon and proofs.

We'll cover:

-   [Random Access Memory](#ram)
-   [Binary Numbers](#binary-numbers)
-   [Fixed-Width Integers](#fixed-width-nums)
-   [Arrays](#arrays)
-   [Strings](#strings)
-   [Pointers](#pointers)
-   [Dynamic Arrays](#dynamic-arrays)
-   [Linked Lists](#linked-lists)
-   [Hash Tables](#hash-tables)

### Get the 7-day crash course!

In this free email course, I'll teach you the right *way of thinking* for breaking down tricky algorithmic coding interview questions.

No CS degree necessary.

<span class="input-group-btn"> </span>

No spam, ever.

**You're in!**

### Get the coding interview crash course

In this free email course, I'll teach you the right *way of thinking* for breaking down tricky algorithmic coding interview questions.

7 days. One short-but-helpful email a day. Unsubscribe whenever.

No CS degree necessary.

No spam, ever. Easy unsubscribe.

You're in! Head over to your email inbox right now to read day one!

## Random Access Memory (RAM)

When a computer is running code, it needs to keep track of *variables* (numbers, strings, arrays, etc.).

Variables are stored in **random access memory** (**RAM**). We sometimes call RAM "working memory" or just "memory."

RAM is *not* where mp3s and apps get stored. In addition to "memory," your computer has **storage** (sometimes called "persistent storage" or "disk"). While *memory* is where we keep the variables our <span words="article__data-structures-coding-interview__function">function</span>s allocate as they crunch data for us, *storage* is where we keep *files* like mp3s, videos, Word documents, and even executable programs or apps.

Memory (or RAM) is faster but has less space, while storage (or "disk") is slower but has more space. A modern laptop might have ~500GB of storage but only ~16GB of RAM.

Think of RAM like a really tall bookcase with a *lot* of shelves. Like, *billions* of shelves.

<img src="/images/svgs/cs_for_hackers__ram_empty_no_indices.svg?bust=209" width="125" height="277" alt="A column of empty RAM slots." />

It just keeps going down. Again, picture *billions* of these shelves.

The shelves are numbered.

<img src="/images/svgs/cs_for_hackers__ram_empty_with_indices.svg?bust=209" width="125" height="277" alt="A column of empty RAM slots with indices." />

We call a shelf's number its **address**.

Each shelf holds 8 **bits**. A *bit* is a tiny electrical switch that can be turned "on" or "off." But instead of calling it "on" or "off" we call it <span code-inline="article__data-structures-coding-interview__one">1</span> or <span code-inline="article__data-structures-coding-interview__zero">0</span>.

<img src="/images/svgs/cs_for_hackers__ram_bits.svg?bust=209" width="125" height="277" alt="A column of RAM slots filled with various bits that make up bytes." />

8 bits is called a **byte**. So each shelf has one byte (8 bits) of storage.

Of course, we also have a processor that does all the real work inside our computer:

<img src="/images/svgs/cs_for_hackers__ram_processor.svg?bust=209" width="309" height="277" alt="A section of RAM connected to the computer&#39;s processor, which does most of the heavy lifting." />

It's connected to a **memory controller**. The memory controller does the actual reading and writing to and from RAM. It has a *direct connection* to each shelf of RAM.

<img src="/images/svgs/cs_for_hackers__ram_memory_controller.svg?bust=209" width="309" height="277" alt="The computer&#39;s processor connected to a memory controller, which does the actual reading and writing to and from RAM." />

That *direct connection* is important. It means we can access address 0 and then immediately access address 918,873 without having to "climb down" our massive bookshelf of RAM.

That's why we call it Random Access Memory (RAM)—we can *Access* the bits at any *Random* address in *Memory* right away.

Spinning hard drives don't have this "random access" superpower, because there's no direct connection to each byte on the disk. Instead, there's a reader—called a **head**—that moves along the surface of a spinning storage disk (like the needle on a record player). Reading bytes that are far apart takes longer because you have to wait for the head to physically move along the disk.

Even though the memory controller can jump between far-apart memory addresses quickly, programs *tend to* access memory that's nearby. **So computers are tuned to get an extra speed boost when reading memory addresses that're close to each other**. Here's how it works:

The processor has a **cache** where it stores a copy of stuff it's recently read from RAM.

<img src="/images/svgs/cs_for_hackers__ram_cache.svg?bust=209" width="309" height="277" alt="A series of caches inside of the memory controller, where the processor stores what it has recently read from RAM." />

Actually, it has a *series* of caches. But we can picture them all lumped together as one cache like this.

This cache is much faster to read from than RAM, so the processor saves time whenever it can read something from cache instead of going out to RAM.

**When the processor asks for the contents of a given memory address, the memory controller *also* sends the contents of a handful of *nearby* memory addresses.** And the processor puts *all* of it in the cache.

So if the processor asks for the contents of address 951, then 952, then 953, then 954...it'll go out to RAM once for that first read, and the subsequent reads will come straight from the super-fast cache.

But if the processor asks to read address 951, then address 362, then address 419...then the cache won't help, and it'll have to go all the way out to RAM for each read.

So reading from sequential memory addresses is faster than jumping around.

## Binary numbers

Let's put those bits to use. Let's store some stuff. Starting with numbers.

The number system we usually use (the one you probably learned in elementary school) is called **base 10**, because each digit has *ten* possible values (1, 2, 3, 4, 5, 6, 7, 8, 9, and 0).

But computers don't have digits with ten possible values. They have *bits* with *two* possible values. So they use **base 2** numbers.

Base 10 is also called **decimal**. Base 2 is also called **binary**.

To understand binary, let's take a closer look at how decimal numbers work. Take the number "101" in decimal:

<img src="/images/svgs/cs_for_hackers__binary_numbers_base_10_101.svg?bust=209" width="115" height="50" alt="In base 10, the digits 101 represent 1 hundred, 0 tens, and 1 one." />

Notice we have two "1"s here, but they don't *mean* the same thing. The leftmost "1" *means* 100, and the rightmost "1" *means* 1. That's because the leftmost "1" is in the hundreds place, while the rightmost "1" is in the ones place. And the "0" between them is in the tens place.

<img src="/images/svgs/cs_for_hackers__binary_numbers_base_10_digits.svg?bust=209" width="341" height="100" alt="In base 10, the digits 101 represent 1 hundred, 0 tens, and 1 one." />

**So this "101" in base 10 is telling us we have "1 hundred, 0 tens, and 1 one."**

<img src="/images/svgs/cs_for_hackers__binary_numbers_base_10.svg?bust=209" width="341" height="199" alt="In base 10, the digits 101 represent 1 hundred, 0 tens, and 1 one, which add to give the value one hundred and one." />

Notice how the *places* in base 10 (ones place, tens place, hundreds place, etc.) are *sequential powers of 10*:

-   <span math=""> 10^0=1 </span>
-   <span math=""> 10^1=10 </span>
-   <span math=""> 10^2=100 </span>
-   <span math=""> 10^3=1000 </span>
-   etc.

**The places in *binary* (base 2) are sequential powers of *2*:**

-   <span math="">2^0=1</span>
-   <span math="">2^1=2</span>
-   <span math="">2^2=4</span>
-   <span math="">2^3=8</span>
-   etc.

So let's take that same "101" but this time let's read it as a *binary* number:

<img src="/images/svgs/cs_for_hackers__binary_numbers_base_2_digits.svg?bust=209" width="341" height="100" alt="In base 2, the digits 101 represent 1 four, 0 twos, and 1 one." />

Reading this from right to left: we have a 1 in the ones place, a 0 in the twos place, and a 1 in the fours place. So our total is 4 + 0 + 1 which is 5.

<img src="/images/svgs/cs_for_hackers__binary_numbers_base_2.svg?bust=209" width="341" height="199" alt="In base 2, the digits 101 represent 1 four, 0 twos, and 1 one, which add to give the value five." />

Here's how we'd count up to 12 in binary:

<table class="table table-condensed binary-table"><thead><tr class="header"><th><strong>Decimal</strong></th><th><strong>Binary</strong></th></tr></thead><tbody><tr class="odd"><td><span data-math="">0</span></td><td class="cl">0000</td></tr><tr class="even"><td><span data-math="">1</span></td><td class="cl">0001</td></tr><tr class="odd"><td><span data-math="">2</span></td><td class="cl">0010</td></tr><tr class="even"><td><span data-math="">3</span></td><td class="cl">0011</td></tr><tr class="odd"><td><span data-math="">4</span></td><td class="cl">0100</td></tr><tr class="even"><td><span data-math="">5</span></td><td class="cl">0101</td></tr><tr class="odd"><td><span data-math="">6</span></td><td class="cl">0110</td></tr><tr class="even"><td><span data-math="">7</span></td><td class="cl">0111</td></tr><tr class="odd"><td><span data-math="">8</span></td><td class="cl">1000</td></tr><tr class="even"><td><span data-math="">9</span></td><td class="cl">1001</td></tr><tr class="odd"><td><span data-math="">10</span></td><td class="cl">1010</td></tr><tr class="even"><td><span data-math="">11</span></td><td class="cl">1011</td></tr><tr class="odd"><td><span data-math="">12</span></td><td class="cl">1100</td></tr></tbody></table>

So far we've been talking about **unsigned integers** ("unsigned" means non-negative, and "integer" means a whole number, not a fraction or decimal). Storing other numbers isn't hard though. Here's how some other numbers *could* be stored:

**Fractions:** Store *two* numbers: the numerator and the denominator.

**Decimals:** Also two numbers: 1) the number with the decimal point taken out, and 2) the *position* where the decimal point goes (how many digits over from the leftmost digit).

**Negative Numbers:** Reserve the leftmost bit for expressing the sign of the number. <span code-inline="article__data-structures-coding-interview__zero">0</span> for positive and <span code-inline="article__data-structures-coding-interview__one">1</span> for negative.

In reality we usually do something slightly fancier for each of these. But these approaches *work*, and they show how we can express some complex stuff with just <span code-inline="article__data-structures-coding-interview__one">1</span>s and <span code-inline="article__data-structures-coding-interview__zero">0</span>s.

We've talked about base 10 and base 2...you may have also seen **base 16**, also called **hexadecimal** or **hex**.

In hex, our possible values for each digit are 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, a, b, c, d, e, and f. Hex numbers are often prefixed with "0x" or "#".

In CSS, colors are sometimes expressed in hex. Interview Cake's signature blue color is "#5bc0de".

## Fixed-width integers

How many different numbers can we express with 1 byte (8 bits)?

<span math="">2^8=256</span> different numbers. <span concept="bits-number-of-possibilities">*How did we know to take <span math="">2^8</span>?*</span>

What happens if we have the number 255 in an 8-bit unsigned integer (<span code-inline="article__data-structures-coding-interview__one-one-one-one-one-one-one-one">1111 1111</span> in binary) and we add 1? The answer (256) needs a 9th bit (<span code-inline="article__data-structures-coding-interview__one-zero-zero-zero-zero-zero-zero-zero-zero">1 0000 0000</span>). But we only have 8 bits!

This is called an **integer overflow**. At best, we might just get an error. At worst, our computer might compute the correct answer but then just throw out the 9th bit, giving us *zero* (<span code-inline="article__data-structures-coding-interview__zero-zero-zero-zero-zero-zero-zero-zero">0000 0000</span>) instead of 256 (<span code-inline="article__data-structures-coding-interview__one-zero-zero-zero-zero-zero-zero-zero-zero">1 0000 0000</span>)! (<span words="article__data-structures-coding-interview__how-overflow-is-handled">Python actually notices that the result won't fit and automatically allocates more bits to store the larger number.</span>)

The 256 possibilities we get with 1 byte are pretty limiting. So **we usually use 4 or 8 bytes (32 or 64 bits) for storing integers**.

-   32-bit integers have <span math="">2^{32}</span> possible values—more than *4 billion*
-   64-bit integers have <span math="">2^{64}</span> possible values—more than *10 billion billion* (<span math="">10^{19}</span>).

**"How come I've never had to think about how many bits my integers are?"** Maybe you *have* but just didn't know it.

Have you ever noticed how in some languages (<span words="article__data-structures-coding-interview__languages-with-different-integer-types">like Java and C</span>) sometimes numbers are <span code-inline="article__data-structures-coding-interview__integer">Integer</span>s and sometimes they're <span code-inline="article__data-structures-coding-interview__long">Long</span>s? The difference is the number of bits (in Java, <span code-inline="article__data-structures-coding-interview__integer">Integer</span>s are 32 bits and <span code-inline="article__data-structures-coding-interview__long">Long</span>s are 64).

Ever created a table in SQL? When you specify that a column will hold integers, you have to specify how many bytes: 1 byte (<span code-inline="article__data-structures-coding-interview__tinyint">tinyint</span>), 2 bytes (<span code-inline="article__data-structures-coding-interview__smallint">smallint</span>), 4 bytes (<span code-inline="article__data-structures-coding-interview__int">int</span>), or 8 bytes (<span code-inline="article__data-structures-coding-interview__bigint">bigint</span>).

**When is 32 bits not enough? When you're counting views on a viral video**. YouTube famously ran into trouble when the Gangnam Style video hit over <span math="">2^{31}</span> views, [forcing them to upgrade their view counts from 32-bit to 64-bit signed integers](http://arstechnica.com/business/2014/12/gangnam-style-overflows-int_max-forces-youtube-to-go-64-bit/).

Most integers are **fixed-width** or **fixed-length**, which means the number of bits they take up doesn't change.

It's usually safe to assume an integer is fixed-width unless you're told otherwise. Variable-size numbers *exist*, but they're only used in special cases.

If we have a 64-bit fixed-length integer, it doesn't matter if that integer is 0 or 193,457—it still takes up the same amount of space in RAM: 64 bits.

**Are you familiar with big O notation?** It's a tool we use for talking about how much time an algorithm takes to run or how much space a data structure takes up in RAM. It's pretty simple:

**<span complexity="1"></span>** or **constant** means the time or space stays about the same even as the dataset gets bigger and bigger.

**<span complexity="n"></span>** or **linear** means the time or space grows proportionally as the dataset grows.

So <span complexity="1"></span> space is much smaller than <span complexity="n"></span> space. And <span complexity="1"></span> *time* is much faster than <span complexity="n"></span> time.

That's all you need for this piece. But if you're curious, you can read [our whole big O explainer here](/big-o-notation-time-and-space-complexity).

In big O notation, we say **fixed-width integers take up *constant space* or <span complexity="1"></span> space.**

And *because* they have a constant number of bits, **most simple operations on fixed-width integers (addition, subtraction, multiplication, division) take constant *time* (<span complexity="1"></span> time)**.

So fixed-width integers are very space efficient and time efficient.

But that efficiency comes at a cost—*their values are limited*. Specifically, they're limited to <span math="">2^n</span> possibilities, where <span math="">n</span> is the number of bits.

So there's a tradeoff. As we'll see, that's a trend in data structures—to get a nice property, we'll often have to lose something.

Real quick—is this making sense? Feeling like it's coming together?

**Keep up the momentum!** Sign up to get a data structures and algorithms practice question sent to you every week.

<span class="input-group-btn"> </span>

No spam, ever. Easy unsubscribe.

*Cool, watch your inbox!*

## Arrays

Ok, so we know how to store individual numbers. Let's talk about storing *several numbers*.

That's right, things are starting to *heat up*.

Suppose we wanted to keep a count of how many bottles of kombucha we drink every day.

Let's store each day's kombucha count in an 8-bit, fixed-width, unsigned integer. That should be plenty—we're not likely to get through more than 256 (<span math="">2^8</span>) bottles in a *single day*, right?

And let's store the kombucha counts right next to each other in RAM, starting at memory address 0:

<img src="/images/svgs/cs_for_hackers__array_kombucha_counts.svg?bust=209" width="250" height="310" alt="A stack of RAM in which we store kombucha counts starting at index 0." />

Bam. That's an **array**. RAM is *basically* an array already.

Just like with RAM, the elements of an array are numbered. We call that number the **index** of the array element (plural: indices). In *this* example, each array element's index is the same as its address in RAM.

But that's not usually true. Suppose another program like Spotify had already stored some information at memory address 2:

<img src="/images/svgs/cs_for_hackers__array5_occupied.svg?bust=209" width="250" height="310" alt="A column of 9 RAM slots representing an array. The row at index 2 is highlighted because it is being used by Spotify." />

We'd have to start our array below it, for example at memory address 3. So index 0 in our array would be at memory address 3, and index 1 would be at memory address 4, etc.:

<img src="/images/svgs/cs_for_hackers__array5.svg?bust=209" width="250" height="350" alt="A column of 9 RAM slots representing an array. The row at index 2 is highlighted, and the rows at indices 3 through 7 are selected with a bracket." />

Suppose we wanted to get the kombucha count at index 4 in our array. How do we figure out what *address in memory* to go to? Simple math:

Take the array's starting address (3), add the index we're looking for (4), and that's the address of the item we're looking for. 3 + 4 = 7. In general, for getting the <span math="">n</span>th item in our array:

<span block="" math=""> \\text{address of nth item in array} = </span> <span block="" math=""> \\text{address of array start} + n </span>

This works out nicely because the size of the addressed memory slots and the size of each kombucha count are *both* 1 byte. So a slot in our array corresponds to a slot in RAM.

But that's not always the case. In fact, it's *usually not* the case. We *usually* use *64-bit* integers.

So how do we build an array of *64-bit* (8 byte) integers on top of our *8-bit* (1 byte) memory slots?

We simply give each array index *8* address slots instead of 1:

<img src="/images/svgs/cs_for_hackers__array64_long.svg?bust=209" width="162" height="433" alt="A column of RAM slots representing an array of 64-bit integers. Every 8 buckets of RAM represents one integer." />

So we can still use simple math to grab the start of the <span math="">nth</span> item in our array—just gotta throw in some multiplication:

<span block="" math=""> \\text{address of nth item in array} = </span> <span block="" math=""> \\text{address of array start} + (n \* \\text{size of each item in bytes}) </span>

Don't worry—adding this multiplication doesn't really slow us down. Remember: addition, subtraction, multiplication, and division of fixed-width integers takes <span complexity="1"></span> time. So *all* the math we're using here to get the address of the <span math="">n</span>th item in the array takes <span complexity="1"></span> time.

And remember how we said the memory controller has a *direct connection* to each slot in RAM? That means we can read the stuff at any given memory address in <span complexity="1"></span> time.

<img src="/images/svgs/cs_for_hackers__arrays_no_processor_ram_memory_controller.svg?bust=209" width="248" height="279" alt="A memory controller connected to a section of RAM." />

**Together, this means looking up the contents of a given array index is <span complexity="1"></span> time.** This fast lookup capability is the most important property of arrays.

But the formula we used to get the address of the <span math="">n</span>th item in our array only works *if*:

1.  **Each item in the array is the *same size*** (takes up the same number of bytes).
2.  **The array is *uninterrupted* (contiguous) in memory**. There can't be any gaps in the array...like to "skip over" a memory slot Spotify was already using.

These things make our formula for finding the <span math="">n</span>th item *work* because they make our array *predictable*. We can *predict* exactly where in memory the <span math="">n</span>th element of our array will be.

But they also constrain what kinds of things we can put in an array. Every item has to be the same size. And if our array is going to store a *lot* of stuff, we'll need a *bunch* of uninterrupted free space in RAM. Which gets hard when most of our RAM is already occupied by other programs (like Spotify).

That's the tradeoff. Arrays have fast lookups (<span complexity="1"></span> time), but each item in the array needs to be the same size, and you need a big block of uninterrupted free memory to store the array.

## Strings

Okay, let's store some words.

A series of *characters* (letters, punctuation, etc.) is called a **string**.

We already know one way to store a *series of things*—arrays. But how can an array store *characters* instead of numbers?

Easy. Let's define a mapping between numbers and characters. Let's say "A" is 1 (or <span code-inline="article__data-structures-coding-interview__zero-zero-zero-zero-zero-zero-zero-one">0000 0001</span> in binary), "B" is 2 (or <span code-inline="article__data-structures-coding-interview__zero-zero-zero-zero-zero-zero-one-zero">0000 0010</span> in binary), etc. Bam. Now we have characters.

This mapping of numbers to characters is called a **character encoding**. One common character encoding is "ASCII". Here's how the alphabet is encoded in ASCII:

A: 01000001

S: 01010011

k: 01101011

B: 01000010

T: 01010100

l: 01101100

C: 01000011

U: 01010101

m: 01101101

D: 01000100

V: 01010110

n: 01111110

E: 01000101

W: 01010111

o: 01101111

F: 01000110

X: 01011000

p: 01110000

G: 01000111

Y: 01011001

q: 01110001

H: 01001000

Z: 01011010

r: 01110010

I: 01001001

a: 01100001

s: 01110011

J: 01001010

b: 01100010

t: 01110100

K: 01001011

c: 01100011

u: 01110101

L: 01001100

d: 01100100

v: 01110110

M: 01001101

e: 01100101

w: 01110111

N: 01001110

f: 01100110

x: 01111000

O: 01001111

g: 01100111

y: 01111001

P: 01010000

h: 01101000

z: 01111010

Q: 01010001

i: 01101001

 

R: 01010010

j: 01101010

 

You get the idea. So since we can express characters as 8-bit integers, we can express *strings* as *arrays* of 8-bit <s>numbers</s> characters.

<img src="/images/svgs/cs_for_hackers__strings_nice_array.svg?bust=209" width="256" height="152" alt="Three illustrations of the string &quot;NICE&quot;: one in binary, one in base 10, and one in ASCII." />

## Pointers

Remember how we said every item in an array had to be the same size? Let's dig into that a little more.

Suppose we wanted to store a bunch of ideas for baby names. Because we've got some *really* cute ones.

Each name is a string. Which is really an array. And now we want to store *those arrays* in an array. *Whoa*.

Now, what if our baby names have different lengths? That'd violate our rule that all the items in an array need to be the same size!

We could put our baby names in arbitrarily large arrays (say, 13 characters each), and just use a special character to mark the end of the string within each array...

<img src="/images/svgs/cs_for_hackers__pointers_baby_names.svg?bust=209" width="262" height="625" alt="Strings represented in RAM as arrays of 13 characters, with the end of the strings being denoted by a special &quot;null&quot; character. The last 8 rows are marked as wasted space because the name Bill (along with the null character) only takes up 5 out of 13 available characters." />

"Wigglesworth" is a cute baby name, right?

But look at all that wasted space after "Bill". And what if we wanted to store a string that was *more* than 13 characters? We'd be out of luck.

There's a better way. Instead of storing the strings right inside our array, let's just put the strings wherever we can fit them in memory. Then we'll have each element in our array hold the *address in memory* of its corresponding string. Each address is an integer, so really our outer array is just an array of integers. We can call each of these integers a **pointer**, since it points to another spot in memory.

<img src="/images/svgs/cs_for_hackers__pointers_pointer_array.svg?bust=209" width="208" height="457" alt="An array of names represented in RAM. The names are stored out of order, but an array holds the address in memory of each of name with arrows pointing from the number to the memory address." />

The pointers are marked with a <span code-inline="article__data-structures-coding-interview__asterisk">\*</span> at the beginning.

Pretty clever, right? This fixes *both* the disadvantages of arrays:

1.  The items don't have to be the same length—each string can be as long or as short as we want.
2.  We don't need enough uninterrupted free memory to store all our strings next to each other—we can place each of them separately, wherever there's space in RAM.

We fixed it! No more tradeoffs. Right?

Nope. Now we have a *new* tradeoff:

Remember how the memory controller sends the contents of *nearby* memory addresses to the processor with each read? And the processor caches them? So reading sequential addresses in RAM is *faster* because we can get most of those reads right from the cache?

<img src="/images/svgs/cs_for_hackers__ram_cache.svg?bust=209" width="309" height="277" alt="A series of caches inside of the memory controller, where the processor stores what it has recently read from RAM." />

Our original array was very **cache-friendly**, because everything was sequential. So reading from the 0th index, then the 1st index, then the 2nd, etc. got an extra speedup from the processor cache.

**But the pointers in this array make it *not* cache-friendly**, because the baby names are scattered randomly around RAM. So reading from the 0th index, then the 1st index, etc. doesn't get that extra speedup from the cache.

That's the tradeoff. This pointer-based array requires less uninterrupted memory and can accommodate elements that aren't all the same size, *but* it's *slower* because it's not cache-friendly.

This slowdown isn't reflected in the big O time cost. Lookups in this pointer-based array are *still* <span complexity="1"></span> time.

## Dynamic arrays

Let's build a very simple word processor. What data structure should we use to store the text as our user writes it?

Strings are stored as arrays, right? So we should use an array?

Here's where that gets tricky: **when we allocate an array in a low-level language like <span words="article__data-structures-coding-interview__language-with-low-level-array">C or Java</span>, we have to specify upfront *how many indices* we want our array to have.**

There's a reason for this—the computer has to reserve space in memory for the array and commit to not letting anything else use that space. We can't have some other program overwriting the elements in our array!

The computer can't reserve *all* its memory for a single array. So we have to tell it how much to reserve.

But for our word processor, we don't know ahead of time how long the user's document is going to be! So what can we do?

Just make an array and program it to resize itself when it runs out of space! This is called a **dynamic array**, and it's built on top of a normal array.

<span words="article__data-structures-coding-interview__languages-with-dynamic-arrays">Python, Ruby, and JavaScript</span> use dynamic arrays for their default array-like data structures. <span words="article__data-structures-coding-interview__what-default-dynamic-arrays-are-called">In Python, they're called "lists."</span> Other languages have both. <span words="article__data-structures-coding-interview__languages-with-both-array-types">For example, in Java, <span code-inline="article__data-structures-coding-interview__array">array</span> is a static array (whose size we have to define ahead of time) and <span code-inline="article__data-structures-coding-interview__array-list">ArrayList</span> is a dynamic array</span>.

Here's how it works:

When you allocate a dynamic array, your dynamic array implementation makes an *underlying static array*. The starting size depends on the implementation—let's say our implementation uses 10 indices:

<img src="/images/svgs/cs_for_hackers__dynamic_arrays_10_indices.svg?bust=209" width="300" height="303" alt="A blank dynamic array created by default with 10 indices." />

Say you append 4 items to your dynamic array:

<img src="/images/svgs/cs_for_hackers__dynamic_arrays_dear.svg?bust=209" width="300" height="303" alt="The same dynamic array storing the word &quot;Dear.&quot;" />

At this point, our dynamic array contains 4 items. It has a length of 4. But the *underlying array* has a length of 10.

We'd say this dynamic array's **size** is 4 and its **capacity** is 10.

<img src="/images/svgs/cs_for_hackers__dynamic_arrays_size_and_capacity.svg?bust=209" width="300" height="303" alt="Our dynamic array now has a size of 4 and a capacity of 10." />

The dynamic array stores an <span var="article__data-structures-coding-interview__end-index">end\_index</span> to keep track of where the dynamic array ends and the extra capacity begins.

<img src="/images/svgs/cs_for_hackers__dynamic_arrays_end_index.svg?bust=209" width="300" height="303" alt="The end_index of our dynamic array is marked at index 3, where the last letter of the word &quot;Dear&quot; is stored." />

If you keep appending, at some point you'll use up the full capacity of the underlying array:

<img src="/images/svgs/cs_for_hackers__dynamic_arrays_array_sweatin.svg?bust=209" width="300" height="303" alt="After adding 6 characters to form the string &quot;Dear Mothe,&quot; the end_index of our dynamic array is now marked at index 9, meaning the dynamic array is full." />

Next time you append, the dynamic array implementation will do a few things under the hood to make it work:

**1. Make a new, bigger array.** Usually twice as big.

Why not just *extend* the existing array? Because that memory might already be taken. Say we have Spotify open and it's using a handful of memory addresses right after the end of our old array. We'll have to skip that memory and reserve the next 20 uninterrupted memory slots for our new array:

<img src="/images/svgs/cs_for_hackers__dynamic_arrays_new_array.svg?bust=209" width="211" height="614" alt="A new dynamic array, twice as big as the old dynamic array, is created in order to make more room." />

**2. Copy *each* element from the old array into the new array.**

<img src="/images/svgs/cs_for_hackers__dynamic_arrays_copy_array.svg?bust=209" width="211" height="614" alt="Each element from the old dynamic array is copied into the new dynamic array." />

**3. Free up the old array.** This tells the operating system, "you can use this memory for something else now."

<img src="/images/svgs/cs_for_hackers__dynamic_arrays_free_old_array.svg?bust=209" width="211" height="614" alt="The old array is forgotten because it is no longer necessary." />

**4. Append your new item.**

<img src="/images/svgs/cs_for_hackers__dynamic_arrays_append_item.svg?bust=209" width="211" height="614" alt="The new element, the letter &quot;r,&quot; is finally appended to our new array." />

We could call these special appends "doubling" appends since they require us to make a new array that's (usually) double the size of the old one.

Appending an item to an array is usually an <span complexity="1"></span> time operation, but **a single doubling append is an <span complexity="n"></span> time operation since we have to copy all <span math="">n</span> items from our array.**

Does that mean an append operation on a dynamic array is always worst-case <span complexity="n"></span> time? Yes. So if we make an empty dynamic array and append <span math="">n</span> items, that has some crazy time cost like <span complexity="n^2"></span> or <span complexity="n!"></span>?!?! Not quite.

While the time cost of each special <span complexity="n"></span> doubling append *doubles* each time, the *number of <span complexity="1"></span> appends* you get until the *next doubling* append *also* doubles. This kind of "cancels out," and we can say <span concept="dynamic-array-amortized-analysis-shorter">each append has an *average* cost or **amortized cost** of <span complexity="1"></span>.</span>

Given this, in industry we usually wave our hands and say dynamic arrays have a time cost of <span complexity="1"></span> for appends, even though strictly speaking that's only true for the *average* case or the *amortized* cost.

In an interview, if we were worried about that <span complexity="n"></span>-time worst-case cost of appends, we might try to use a normal, non-dynamic array.

**The *advantage* of dynamic arrays over arrays is that you don't have to specify the size ahead of time, but the *disadvantage* is that some appends can be expensive**. That's the tradeoff.

But what if we wanted the best of both worlds...

## Linked lists

Our word processor is definitely going to need fast appends—appending to the document is like the *main thing* you do with a word processor.

Can we build a data structure that can store a string, has fast appends, *and* doesn't require you to say how long the string will be ahead of time?

Let's focus first on not having to know the length of our string ahead of time. Remember how we used *pointers* to get around length issues with our array of baby names?

What if we pushed that idea even further?

What if each *character* in our string were a *two-index array* with:

1.  the character itself
2.  a pointer to the next character

<img src="/images/svgs/cs_for_hackers__linked_lists_sample.svg?bust=209" width="61" height="327" alt="An example of a linked list storing the string &quot;DEAR.&quot; Each element of the linked list is an array composed of two items: a character and a pointer that points to the next element." />

We would call each of these two-item arrays a **node** and we'd call this series of nodes a **linked list**.

Here's how we'd actually implement it in memory:

<img src="/images/svgs/cs_for_hackers__linked_lists_in_memory.svg?bust=209" width="129" height="409" alt="The same linked list represented in RAM, showing the nodes scattered in memory but connected by pointers." />

Notice how we're free to store our nodes wherever we can find two open slots in memory. They don't have to be next to each other. They don't even have to be *in order*:

<img src="/images/svgs/cs_for_hackers__linked_lists_in_memory_out_of_order.svg?bust=209" width="129" height="409" alt="The same linked list represented in RAM. This time the characters are stored out of order to show that the pointers still keep everything in place." />

"But that's not cache-friendly," you may be thinking. Good point! We'll get to that.

The first node of a linked list is called the **head**, and the last node is usually called the **tail**.

Confusingly, some people prefer to use "tail" to refer to *everything after the head* of a linked list. In an interview it's fine to use either definition. Briefly say which definition you're using, just to be clear.

It's important to have a pointer variable referencing the head of the list—otherwise we'd be unable to find our way back to the start of the list!

We'll also sometimes keep a pointer to the tail. That comes in handy when we want to add something new to the end of the linked list. In fact, let's try that out:

Suppose we had the string "LOG" stored in a linked list:

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string.svg?bust=209" width="141" height="299" alt="A linked list with head and tail pointers storing the word &quot;LOG.&quot; The *head points to the first character &quot;L,&quot; and the tail points to the last letter &quot;G.&quot;" />

Suppose we wanted to add an "S" to the end, to make it "LOGS". How would we do that?

Easy. We just put it in a new node:

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string_add_node.svg?bust=209" width="200" height="390" alt="A linked list with head and tail pointers storing the word &quot;LOG.&quot; A new unconnected node storing the character &quot;S&quot; is added to the bottom and bolded." />

And tweak some pointers:

1\. Grab the last letter, which is "G". Our <span var="article__data-structures-coding-interview__tail">tail</span> pointer lets us do this in <span complexity="1"></span> time.

<img src="/images/svgs/cs_for_hackers__linked_lists_logs_string_grab_last_letter.svg?bust=209" width="200" height="390" alt="A linked list with head and tail pointers storing the word &quot;LOG.&quot; The *tail pointer and the character &quot;G&quot; are bolded." />

2\. Point the last letter's <span var="article__data-structures-coding-interview__next">next</span> to the letter we're appending ("S").

<img src="/images/svgs/cs_for_hackers__linked_lists_logs_string_point_next.svg?bust=209" width="200" height="390" alt="A linked list with head and tail pointers storing the word &quot;LOG.&quot; The &quot;G&quot;&#39;s *next pointer is bolded and pointing to the appended &quot;S&quot;." />

3\. Update the <span var="article__data-structures-coding-interview__tail">tail</span> pointer to point to our *new* last letter, "S".

<img src="/images/svgs/cs_for_hackers__linked_lists_logs_string_tweak_pointers.svg?bust=209" width="200" height="390" alt="A linked list with head and tail pointers storing the word &quot;LOGS.&quot; The *tail pointer is now pointed to the new last letter: &quot;S&quot;." />

That's <span complexity="1"></span> time.

Why is it <span complexity="1"></span> time? Because the runtime doesn't get bigger if the string gets bigger. No matter how many characters are in our string, we still just have to tweak a couple pointers for any append.

Now, what if instead of a linked list, our string had been a *dynamic array*? We might not have any room at the end, forcing us to do one of those doubling operations to make space:

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string_doubled_array.svg?bust=209" width="231" height="188" alt="A dynamic array containing the word &quot;LOG&quot; going through a doubling operation to make space for an appended letter." />

So with a dynamic array, our append would have a *worst-case* time cost of <span complexity="n"></span>.

**Linked lists have worst-case <span complexity="1"></span>-time appends, which is better than the worst-case <span complexity="n"></span> time of dynamic arrays.**

That *worst-case* part is important. The *average case* runtime for appends to linked lists and dynamic arrays is the same: <span complexity="1"></span>.

Now, what if we wanted to *pre*pend something to our string? Let's say we wanted to put a "B" at the beginning.

For our linked list, it's just as easy as appending. Create the node:

<img src="/images/svgs/cs_for_hackers__linked_lists_logs_string_add_node.svg?bust=209" width="200" height="478" alt="A linked list with head and tail pointers storing the word &quot;LOGS.&quot; A new unconnected node storing the character &quot;B&quot; is added to the top and bolded." />

And tweak some pointers:

1.  Point "B"'s <span var="article__data-structures-coding-interview__next">next</span> to "L".
2.  Point the <span var="article__data-structures-coding-interview__head">head</span> to "B".

<img src="/images/svgs/cs_for_hackers__linked_lists_blogs_string_tweak_pointers.svg?bust=209" width="200" height="478" alt="A linked list with head and tail pointers storing the word &quot;LOGS.&quot; The &quot;B&quot;&#39;s *next pointer is bolded and pointing to the letter &quot;L,&quot; and the *head pointer is bolded and pointing to the prepended letter &quot;B&quot;." />

Bam. <span complexity="1"></span> time again.

But if our string were a *dynamic array*...

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string_dynamic_array.svg?bust=209" width="210" height="152" alt="A dynamic array storing the string &quot;LOGS.&quot;" />

And we wanted to add in that "B":

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string_dynamic_array_add_b.svg?bust=209" width="210" height="182" alt="A dynamic array storing the string &quot;LOGS.&quot; A bolded &quot;B&quot; is added above the array." />

Eep. We have to *make room* for the "B"!

We have to move *each character* one space down:

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string_dynamic_array_move_s.svg?bust=209" width="210" height="182" alt="A dynamic array storing the string &quot;LOGS&quot; with the letter &quot;B&quot; floating above. The &quot;S&quot; is bolded with an arrow attached showing how the character is being moved one index up." />

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string_dynamic_array_move_g.svg?bust=209" width="210" height="182" alt="A dynamic array storing the string &quot;LOGS&quot; with the letter &quot;B&quot; floating above. The &quot;G&quot; is bolded with an arrow attached showing how the character is being moved one index up." />

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string_dynamic_array_move_o.svg?bust=209" width="210" height="182" alt="A dynamic array storing the string &quot;LOGS&quot; with the letter &quot;B&quot; floating above. The &quot;O&quot; is bolded with an arrow attached showing how the character is being moved one index up." />

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string_dynamic_array_move_l.svg?bust=209" width="210" height="182" alt="A dynamic array storing the string &quot;LOGS&quot; with the letter &quot;B&quot; floating above. The &quot;L&quot; is bolded with an arrow attached showing how the character is being moved one index up." />

*Now* we can drop the "B" in there:

<img src="/images/svgs/cs_for_hackers__linked_lists_log_string_dynamic_array_chars_moved.svg?bust=209" width="210" height="182" alt="A dynamic array storing the string &quot;LOGS&quot; with the letter &quot;B&quot; floating above. The &quot;B&quot; is bolded with an arrow attached showing how the character is now being placed in the first index." />

What's our time cost here?

It's all in the step where we made room for the first letter. We had to move *all <span math="">n</span>* characters in our string. One at a time. That's <span complexity="n"></span> time.

**So linked lists have faster *pre*pends (<span complexity="1"></span> time) than dynamic arrays (<span complexity="n"></span> time).**

No "worst case" caveat this time—prepends for dynamic arrays are *always* <span complexity="n"></span> time. And prepends for linked lists are *always* <span complexity="1"></span> time.

These quick appends and prepends for linked lists come from the fact that linked list nodes can go anywhere in memory. They don't have to sit right next to each other the way items in an array do.

So if linked lists are so great, why do we usually store strings in an array? **Because [arrays have <span complexity="1"></span>-time lookups](#constant-time-array-lookups).** And those constant-time lookups *come from* the fact that all the array elements are lined up next to each other in memory.

Lookups with a linked list are more of a process, because we have no way of knowing where the <span math="">i</span>th node is in memory. So we have to walk through the linked list node by node, counting as we go, until we hit the <span math="">i</span>th item.

def get\_ith\_item\_in\_linked\_list(head, i): if i &lt; 0: raise ValueError("i can't be negative: %d" % i) current\_node = head current\_position = 0 while current\_node: if current\_position == i: # Found it! return current\_node # Move on to the next node current\_node = current\_node.next current\_position += 1 raise ValueError('List has fewer than i + 1 (%d) nodes' % (i + 1))

That's <span math="">i + 1</span> steps down our linked list to get to the <span math="">i</span>th node (we made our <span words="article__data-structures-coding-interview__function">function</span> zero-based to match indices in arrays). **So linked lists have <span complexity="i"></span>-time lookups.** Much slower than the <span complexity="1"></span>-time lookups for arrays and dynamic arrays.

Not only that—**walking down a linked list is *not* cache-friendly.** Because the next node could be *anywhere* in memory, we don't get any benefit from the processor cache. This means lookups in a linked list are even slower.

So the tradeoff with linked lists is they have faster prepends and faster appends than dynamic arrays, *but* they have slower lookups.

## Hash tables

Quick lookups are often really important. For that reason, we tend to use arrays (<span complexity="1"></span>-time lookups) much more often than linked lists (<span complexity="i"></span>-time lookups).

For example, suppose we wanted to count how many times each ASCII character appears in [Romeo and Juliet](https://raw.githubusercontent.com/GITenberg/The-Tragedy-of-Romeo-and-Juliet_1112/master/1112.txt). How would we store those counts?

We can use arrays in a clever way here. Remember—characters are just numbers. In ASCII (a common character encoding) 'A' is 65, 'B' is 66, etc.

So we can use the character('s number value) as the *index* in our array, and store the *count* for that character *at that index* in the array:

<img src="/images/svgs/cs_for_hackers__hash_tables_chars_to_ints.svg?bust=209" width="407" height="218" alt="An array showing indices 63 through 68. To the left of the indices are the ASCII characters that correspond to the numeric indices with arrows pointing from each character to its corresponding number." />

With this array, we can look up (and edit) the count for any character in constant time. Because we can access any index in our array in constant time.

Something interesting is happening here—this array isn't just a list of values. This array is storing *two* things: characters and counts. The characters are *implied* by the indices.

**So we can think of an array as a *table* with *two columns*...except you don't really get to pick the values in one column (the indices)—they're always 0, 1, 2, 3, etc.**

But what if we wanted to put *any* value in that column and still get quick lookups?

Suppose we wanted to count the number of times each *word* appears in Romeo and Juliet. Can we adapt our array?

Translating a *character* into an array index was easy. But we'll have to do something more clever to translate a *word* (a string) into an array index...

<img src="/images/svgs/cs_for_hackers__hash_tables_lies_key_unlabeled.svg?bust=209" width="406" height="255" alt="A blank array except for the value 20 stored at index 9. To the left the array is the word &quot;lies&quot; with an arrow pointing to the right at diamond with a question mark in the middle. The diamond points to the 9th index of the array." />

Here's one way we could do it:

Grab the number value for each character and add those up.

<img src="/images/svgs/cs_for_hackers__hash_tables_lies_chars.svg?bust=209" width="201" height="79" alt="The word &quot;lies&quot; in quotes. Arrows point from each character down to their corresponding number values, which are separated by plus signs and shown in sum to equal 429." />

The result is 429. But what if we only have *30* slots in our array? We'll use a common trick for forcing a number into a specific range: the <span concept="modulus">modulus operator (<span code-inline="article__data-structures-coding-interview__modulus">%</span>).</span> Modding our sum by 30 ensures we get a whole number that's less than 30 (and at least 0):

429 \\: \\% \\: 30 = 9

Bam. That'll get us from a word (or any string) to an array index.

This data structure is called a **hash table** or **hash map**. In our hash table, the *counts* are the **values** and the *words* ("lies," etc.) are the **keys** (analogous to the *indices* in an array). The process we used to translate a key into an array index is called a **hashing <span words="article__data-structures-coding-interview__function">function</span>**.

<img src="/images/svgs/cs_for_hackers__hash_tables_lies_key_labeled.svg?bust=209" width="407" height="254" alt="A blank array except for a 20, labeled as the value, stored at index 9. To the left the array is the word &quot;lies,&quot; labeled as the key, with an arrow pointing to the right at diamond with a question mark in the middle, labeled as the hashing function. The diamond points to the 9th index of the array." />

The hashing <span words="article__data-structures-coding-interview__function">function</span>s used in modern systems get pretty complicated—the one we used here is a simplified example.

Note that our quick lookups are only in one direction—we can quickly get the value for a given key, but the only way to get the key for a given value is to walk through all the values and keys.

Same thing with arrays—we can quickly look up the value at a given index, but the only way to figure out the index for a given value is to walk through the whole array.

One problem—what if two keys hash to the same index in our array? Look at "lies" and "foes":

<img src="/images/svgs/cs_for_hackers__hash_tables_lies_and_foes_addition.svg?bust=209" width="226" height="171" alt="The word &quot;lies&quot; in quotes and the word &quot;foes&quot; in quotes. Arrows point from the characters of each word to their corresponding number values. The sum of the characters of both words is shown to equal 429." />

They both sum up to 429! So of course they'll have the same answer when we mod by 30:

429 \\: \\% \\: 30 = 9

So our hashing <span words="article__data-structures-coding-interview__function">function</span> gives us the same answer for "lies" and "foes." This is called a **hash collision**. There are a few different strategies for dealing with them.

Here's a common one: instead of storing the actual values in our array, let's have each array slot hold a *pointer* to a *linked list* holding the counts for all the words that hash to that index:

<img src="/images/svgs/cs_for_hackers__hash_tables_hash_collision.svg?bust=209" width="322" height="254" alt="An array storing pointers. Three of the pointers have arrows pointing to linked lists to the right of the array." />

One problem—how do we know which count is for "lies" and which is for "foes"? To fix this, we'll store the *word* as well as the count in each linked list node:

<img src="/images/svgs/cs_for_hackers__hash_tables_hash_collision_key_val.svg?bust=209" width="322" height="254" alt="An array storing pointers. The pointer at index 9 has an arrow pointing to a linked list to the right of the array. Each linked list node now stores the word as well as its count and a pointer." />

"But wait!" you may be thinking, "Now lookups in our hash table take <span complexity="n"></span> time in the worst case, since we have to walk down a linked list." That's true! You could even say that in the worst case *every* key creates a hash collision, so our whole hash table *degrades to a linked list*.

In industry though, we usually wave our hands and say **collisions are rare enough that on *average* lookups in a hash table are <span complexity="1"></span> time**. And there are fancy algorithms that keep the number of collisions low and keep the lengths of our linked lists nice and short.

But that's sort of the tradeoff with hash tables. You get fast lookups by key...except *some* lookups could be slow. And of course, you only get those fast lookups in one direction—looking up the *key* for a given *value* still takes <span complexity="n"></span> time.

## Summary

**Arrays** have <span complexity="1"></span>-time lookups. But you need enough *uninterrupted* space in RAM to store the whole array. And the array items need to be the same size.

But if your array stores **pointers** to the actual array items (like we did with our list of baby names), you can get around both those weaknesses. You can store each array item wherever there's space in RAM, and the array items can be different sizes. The tradeoff is that now your array is *slower* because it's not cache-friendly.

Another problem with arrays is you have to specify their sizes ahead of time. There are two ways to get around this: **dynamic arrays** and **linked lists**. Linked lists have faster appends and prepends than dynamic arrays, but dynamic arrays have faster lookups.

Fast lookups are really useful, especially if you can look things up not just by *indices* (0, 1, 2, 3, etc.) but by arbitrary *keys* ("lies", "foes"...any *string*). That's what **hash tables** are for. The only problem with hash tables is they have to deal with hash collisions, which means *some* lookups *could* be a bit slow.

**Each data structure has tradeoffs. You can't have it all.**

So you have to know *what's important* in the problem you're working on. What does your data structure need to do *quickly*? Is it lookups by index? Is it appends or prepends?

Once you know what's important, you can pick the data structure that does it best.

<a href="https://www.facebook.com/sharer/sharer.php?u=https%3A//www.interviewcake.com/article/python/data-structures-coding-interview%3Fcourse%3Ddsa%0A%0A" class="custom-share facebook-share"><em></em> Share</a> <a href="https://twitter.com/intent/tweet?text=Data%20Structures%20for%20Coding%20Interviews%3A%20No%20computer%20science%20knowledge%20necessary&amp;via=interviewcake&amp;related=interviewcake&amp;url=https%3A//www.interviewcake.com/article/python/data-structures-coding-interview%3Fcourse%3Ddsa%0A" class="custom-share twitter-share"><em></em> Tweet</a>

<span class="back-to"> [<span class="glyphicon glyphicon-arrow-left"></span> The Intuitive Guide to Data Structures and Algorithms](/data-structures-and-algorithms-guide) </span> <span class="next"> Next up: [Logarithms <span class="glyphicon glyphicon-arrow-right"></span>](/article/logarithms?course=dsa) </span>

## AHHH I can't read all this right now!

Get The Data Structures and Algorithms Guide sent to you as a set of bite-size readings. We'll send you one a day for about a week.

<span class="input-group-btn"> </span>

No spam, ever. Easy unsubscribe.

**Sweet! We'll send you the first bite-size chunk soon :)**

Want more coding interview help?

Check out <span class="url">interviewcake.com</span> for more advice, guides, and practice questions.

<a href="/free-weekly-coding-interview-problem-newsletter" class="newsletter-link">Subscribe to our weekly question email list »</a>

##### Programming interview questions by company:

-   [Google interview questions](/google-interview-questions)
-   [Facebook interview questions](/facebook-interview-questions)
-   [Amazon interview questions](/amazon-interview-questions)
-   [Uber interview questions](/uber-interview-questions)
-   [Microsoft interview questions](/microsoft-interview-questions)
-   [Apple interview questions](/apple-interview-questions)
-   [Netflix interview questions](/netflix-interview-questions)
-   [Dropbox interview questions](/dropbox-interview-questions)
-   [eBay interview questions](/ebay-interview-questions)
-   [LinkedIn interview questions](/linkedin-interview-questions)
-   [Oracle interview questions](/oracle-interview-questions)
-   [PayPal interview questions](/paypal-interview-questions)
-   [Yahoo interview questions](/yahoo-interview-questions)

##### Programming interview questions by topic:

-   [SQL interview questions](/sql-interview-questions)
-   [Testing and QA interview questions](/testing-and-qa-interview-questions)
-   [Bit manipulation interview questions](/bit-manipulation)
-   [Java interview questions](/java-interview-questions)
-   [Python interview questions](/python-interview-questions)
-   [Ruby interview questions](/ruby-interview-questions)
-   [JavaScript interview questions](/javascript-interview-questions)
-   [C++ interview questions](/cpp-interview-questions)
-   [C interview questions](/c-interview-questions)
-   [Swift interview questions](/swift-interview-questions)
-   [Objective-C interview questions](/objective-c-interview-questions)
-   [PHP interview questions](/php-interview-questions)
-   [C# interview questions](/c-sharp-interview-questions)

<a href="https://www.facebook.com/interviewcake" class="facebook"><em></em></a> <a href="https://www.twitter.com/interviewcake" class="twitter"><em></em></a>

Copyright © 2021 <span itemprop="name">Cake Labs, Inc.</span> All rights reserved.

<span itemprop="streetAddress">228 Park Ave S #82632</span>, <span itemprop="addressLocality">New York</span>, <span itemprop="addressRegion">NY</span> <span itemprop="addressCountry">US</span> <span itemprop="postalCode">10003</span> <span itemprop="telephone">(862) 294-2956</span>

[About](/about) | [Privacy](/privacy-policy) | [Terms](/terms-and-conditions)

{"id":22442089,"username":"2021-10-13\_15:26:05\_^@i\*2t","email":null,"date\_joined":"2021-10-13T15:26:05.399004+00:00","first\_name":"","last\_name":"","full\_name":"","short\_name":"friend","is\_anonymous":true,"is\_on\_last\_question":false,"percent\_done":0,"num\_questions\_done":0,"num\_questions\_remaining":46,"is\_full\_access":false,"is\_student":false,"first\_payment\_date":null,"last\_payment\_date":null,"num\_free\_questions\_left":3,"terms\_has\_agreed\_to\_latest":false,"preferred\_content\_language":"","preferred\_editor\_language":"","is\_staff":false,"auth\_providers\_human\_readable\_list":"","num\_auth\_providers":0,"auth\_email":""}

×

### Log in/sign up

With just a couple clicks.

<span class="btn btn-soc-github btn-login-btn"> <span class="bar">|</span> <span class="company">GitHub Auth</span></span> <span class="btn btn-soc-google-plus btn-login-btn"> <span class="bar">|</span> <span class="company">Google Auth</span></span> <span class="btn btn-soc-facebook btn-login-btn"> <span class="bar">|</span> <span class="company">Facebook Auth</span></span>

<span class="small">We'll never post on your wall or message your friends.</span>

<span class="small">[Where do I enter my password?](#passwordInfo)</span>

Actually, **we don't support password-based login.** Never have. Just the OAuth methods above. Why?

It's easy and quick. No "reset password" flow. No password to forget.

It lets us avoid storing passwords that hackers could access and use to try to log into our users' email or bank accounts.

It makes it harder for one person to share a paid Interview Cake account with multiple people.

<span class="text text-with-image"> <span class="quotation-mark">“</span>Practice at Interview Cake is the most worthy investment I've ever made. <span class="author"> — Kai </span> </span>

. . .
