# reading-viewing-notes
Notes on articles and videos

### 24-08-2019
#### [Introduction to Vega-Lite][12]
Encoding channels 

[12]: https://vega.github.io/vega-lite/tutorials/getting_started.html

### 23-08-2019

#### [Derek Jones - Finding the gold nugget papers in software engineering research][9]
_The huge number of papers describing failed projects and/or containing clueless nonsense is a major obstacle for anyone wanting to locate useful new knowledge._ Contains some suggestions on quickly evaluating papers as potentially interesting for study, linking to earlier blog posts which dig deeper into certain "research smells".

#### [Philip Wadler - Theorems for free!][10]
Shows how we can derive certain theorems purely from the type signature of functions. Reminded me of parts of the ["Throw Away the Irrelevant" episode of the CoRecursive podcast][11], where they discuss "reasoning about polymorphic type signatures".


[9]: http://ecee.colorado.edu/ecen5533/fall11/reading/free.pdf
[10]: https://corecursive.com/009-throw-away-the-irrelevant-with-john-a-de-goes/
[11]: http://shape-of-code.coding-guidelines.com/2016/06/10/finding-the-gold-nugget-papers-in-software-engineering-research/


### 13-08-2019
#### [Graham Lee - The problem with not-Apple][5] (Blog Post)
Describes NeXTSTEP as a compromise between the vision of the [Xerox Alto](https://en.wikipedia.org/wiki/Xerox_Alto), such as OOP, ethernet and laser printers, and actual available technology of the day such as Display PostScript, UNIX, GNU, and C.

Apple has a certain consistency in the way libraries are organised around "kits" (the groupings of APIs for different applications) and the core Objective-C libraries, compared to the chaos of supporting all the possible combinations of technologies Linux users might have on their systems. But, on closer inspection, maybe the Apple ecosystem isn't so coherent after all (inconsistencies in function call styles in ObjC APIs, Dashboard widgets written in JS)

#### [Graham Lee - Resolution: Subscribe Self][6] (Blog Post)
Discusses using RSS over social media to improve the ratio of interesting to rubbish content we come across.

I'm giving ago, just created my Feedly account and imported Graham's OPML. Let's see how it goes.

#### [Graham Lee - This is fine][7] (Blog Post)
Points out how even when we try and make things "simple" for kids, there's a huge amount of implicit knowledge required (randint means random integer, what's an integer anyway?) even once you have you environment set up which requires an arcane series of steps in itself.

#### [Graham Lee - By the river][8] (Blog Post)
Moving post about mental health and living with negative thoughts.

[5]: https://www.sicpers.info/2017/01/the-problem-with-not-apple/
[6]: http://www.sicpers.info/2017/01/resolution-subscribe-self/
[7]: https://www.sicpers.info/2016/12/this-is-fine/
[8]: https://www.sicpers.info/2016/12/by-the-river/

### 12-08-2019
#### [Greg Wilson - What We Actually Know About Software Development, and Why We Believe It’s True][0] (Conference Talk)

Humourous talk about the importance of applying the scientific method to the ways we work.

- [Cochrane (the Cochrane Collaboration)][1] which organises medical research findings and makes data available to policy-makers and researchers.
- Martin Fowler, who the speaker respects as a thinker of software design, published an article on DSLs in IEEE Software claiming "improved productivity and communication", but the article contains no citations.
- Scottish verdicts: innocent, guilty or unproven.
- Mentions Scott Berkun books with anecdotes about New Guinea
- Aranda & Easterbrook (2005) "Anchoring and Adjustment in Software Estimation". A hint in a spec document about estimated delivery time is the only significant factor for determining what estimates people gave.
- Sackman, Erikson, and Grant (1968): "Exploratory experimental studies comparing online and offline programming performance." The origin of the 10xer myth? This was one afternoon of programming by 12 amateurs. Next major study in the 1980's was 1 hour of programming with 54 programmers.
- Lutz Prechelt instead shows that productivity and reliability depend on the length of the program text. Output LOC is constant independent on level of abstraction, so we should use the highest-level language available to us?
- Boehm et al (1975): "Some Experience with Automated Aids to the Design of Large-Scale Reliable Software." Most errors are introduced in requirements analysis and design, the later they are removed, the more expensive it is. "Pessimists vs Optimists" / "Traditionalists vs Agilistas": do we invest more to eliminate the errors up front, or do we shrink the cycle so bugs are discovered earlier.
- Ceci & Williams: "Why aren't more women in science? Top researchers debate the evidence." The Susan Dweck Effect: praise for effort vs praise for aptitude.
- Standish Group - Chaos Report: about the proportion of software projects that fail and why.
- Fagan 1975: Rigourous inspections can remove 60%-90% of errors before the first test is run. Spend more time reviewing and less time writing unit tests? The first reader and the first hour are the most significant.
- Nagappan et al (2007) & Bird et al (2009): Colocation doesn't correlate with fewer bugs.
- El Emam et al (2001): "The Confounding Effect of Class Size on the Validity of Object-Oriented Metrics": Most metrics' values increate with code size. If you do a double-barrelled correlation, the latter accounts for all the signal.
- Andy Oram, Greg Wilson (2007): Beautiful Code: Leading Programmers Explain How They Think
- Andy Oram, Greg Wilson (2010): Making Software: What Really Works, and Why We Believe It
- Edward Tufte: Beautiful Evidence

Talk ends with a plea to use evidence-based policy, and evidence-based approaches in general.

#### [Scott Berkun - Myths of Innovation][4]

Innovation requires graft, the supposed epiphany moments (eureka, Newton's apple) are seductive because they absolve us of our responsibility to put in the work required to make breakthroughs. Also, ability to fail is important. A lot of what we know about history is trivia rather than fact-based stories which would allow us to understand the processes involved. After Richard Drew's masking tape breakthough, 3M realised that delegation of responsibility and the freedom to experiment and mistakes are a necessary part of the innovation and William McKnight recognised his own shortcomings and enshrined that in the company values.

#### [Graham Lee - Why your app is not massively parallel software][2] (Blog Post)
Why your app is not massively parallel software

- Mentions the `#pragma omp parallel for` from [OpenMP][3]. 
- Claims there is a lack of applications taking advantange of the parallel processing capabilities of the Mac Pro.
- Also that the reality of adapting your application design to take advantage of OpenCL doesn't pay off in terms of sufficient performance improvements.
- The libraries and tools that programmers have to support parallelism are inadequate, they should automatically detect opportunities to parallelise work.


[0]: https://vimeo.com/9270320
[1]: https://en.wikipedia.org/wiki/Cochrane_(organisation)
[2]: https://www.sicpers.info/2017/04/why-your-app-is-not-massively-parallel-software/
[3]: https://en.wikipedia.org/wiki/OpenMP
[4]: https://www.youtube.com/watch?v=amt3ag2BaKc
