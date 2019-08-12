# reading-viewing-notes
Notes on articles and videos


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
- Beautiful Code: Leading Programmers Explain How They Think
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
