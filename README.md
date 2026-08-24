# CS50x Blog
Here I'm going to log everyday of my experience taking the CS50x course.

### Day 32: August 23, 2026
**Today's Progress**: almost finished re watching the lecture of week 6 on python.
**Thoughts**: i should have just skipped to the 1h30m mark but i started from the beginning and it took me multiple hours to get to where it was useful to rewatch and write the code being taught. but i think i am getting good practice.

### Day 31: August 19, 2026
**Today's Progress**: solved until credit of week 6
**Thoughts**: hello, mario, cash. all were easy and i felt great until credit. i finally understood how good of a problem credit was all this time. it's simple to understand by writing a good structure answer is where it really shines. despite this time being python i kept thinking in my old manners. and when i decided to take a look at the c code i wrote, i realised this was what the ai suggested as an improvement to my really bad code. it also taught me a really good lesson, humans might the biggest factor in what code gets written in the real world. because code has to be readable first, it can be slow, today we can afford it to be slow. it would be an absolute nightmare to always write the best possible code, it will not work in a group setting. code will always be written for the last performing person in the group. anyway, it was fun. i had a bug where i used an extra > infront of = in an if condition and it took me 30 to debug it. debugging as you write code is the way but it gets harder and harder to do it as the line get into the thousands. the biggest difference in how good of a programmer someone can be will be experience, every one has access to educational resources but who applies them over and over? very few. 

### Day 30: August 17, 2026
**Today's Progress**: watched Week 6 lecture on python.
**Thoughts**: I saw so many comments saying they are happy that C is finally done and python feels great. but i feel the opposite, it was sad to let c go. and i find the python's simple code unnecessary. really got me questioning how do new languages get popular, what drives it, i think it is the median engineer that drives it, assuming the managers generally are not the most competent engineers themself ofcourse they prefer an easier language to write in and more importantly to review. i imagine it is harder to review c or cpp code than python or java. anyway, i think i will get used to python and then appreciate it, until then i have to keep an open mind. now that i miss c, i will definitely go read the c programming language book and do a few projects at least to enjoy it. 

### Day 29: August 15, 2026
**Today's Progress**: solved week 5 speller problem.
**Thoughts**: after a week of kicking myself to solve i finally did it. and to my surprise it was not so hard. I was very scared to attempt the problem. all the scary code in the speller.c file did not help. if i have to point to one major problem i faced, that would be not knowing the flow of code. there were 5 functions we were suppose to write. and if i knew how it's all connected in code, it would have removed great amount of confusion. other than that, AI again help me a great deal, i asked it to review before compiling, it pointed to some syntax blunders but at the end it came up with some bullshit, this was the first time it happened to me and i will have to watch out. it told me it would take 10 to 13 hours to finish this but honestly if i attempted it in one sitting, i think i could've solved in 3 hours. i took 5 hours, 2 hours watching the walkthrough multiple times and 3 hours writing code. off to the rest of the course, i think it will be easier from here. if i were to write an auto complete for phone typing, i would know what to do. if i made the dictionary size smaller to what most people type most of the time, i think the program can give suggestion within 1 second, which is impressive. 

### Day 28: August 7, 2026
**Today's Progress**: started solving week 5 speller problem.
**Thoughts**: i watched the walkthrough of this problem about 3 times and then once more while writing code. the distribution code looks like its beyond my comprehension. i know, i'm not expected to understand but it feels good when i take a glance under the hood. 

### Day 27: August 6, 2026
**Today's Progress**: rewrote linked list & solved week 5 inheritance problem.
**Thoughts**: pointers are confusing. even after successfully rewriting linked list all by my self. i made a few mistakes ofcourse. because a linked list goes only in one direction, if you have insert a node in between, you can only do so between the next node and the one next to it as you only have a pointer to node, with no recourse to the previous one. it's very hard to learn something without breaking it apart and failing to put it back. but it's a lot of fun. one thing i noticed is that there are multiple layers when dealing with pointers. first there is a variable by some name that is of pointer type. this pointer also has a memory address of its own. this pointer points to an address in memory. that has a name, a type also along with contents inside it. you can access these contents using dereferencing. getting all of this down and the interaction among all  of the elements of code takes time and practice, a lot more than waht cs50 offers.
Now, Inheritance was hard. it is hard to imagine how to access pointers, multiple of them, on top of recursion. and then to go back and free up the memory, its very challenging. Gemini told me it is relatively easy and will take two hours. it took 2 hours, i spent 1 hour just rewatching the guide video. tomorrow i will try to write the code from scratch.

### Day 26: August 04, 2026
**Today's Progress**: finished week 5 lecture.
**Thoughts**: That was a lot. it took me two days of 4hours to finish the lecture and rewatch the bits where i had confusion and rewriting the linked list code from despite having a look at the code from the class, it was tough even then. 

### Day 25: August 02, 2026
**Today's Progress**: watched around 1 hour of week 5 lecture.
**Thoughts**: and now the lectures are getting hard to follow. or maybe it's because it's pointers in C. i hope its the later. as if pointers are not hard enough to follow, now i get what's memory management and why it's hard. actually i'm starting to get why programming is hard as i can see what contributes to the complexity. anyway, the linked list of today's lecture was by far the most interesting topic explained so far as it amps up the complexity by multiple degrees. i'll try to rewrite the linked list code from the lecture before going any further. one interesting doubt i had was that with the code david write where he iterates a linked list through 3 user inputed ints, i feel that the first node has the address of the first n through link address in the ->next. but david says it is NULL, which is interesting. i'll ask AI when i rewrite the code tomorrow. 

### Day 24: July 30, 2026
**Today's Progress**: solved recover of week 4.
**Thoughts**: Definitely not as easy as i expected it yesterday. It took me a while to write the code. first i tried to include the first JPEG case inside the while loop but i felt why should the code check everytime if it's the first JPEG, its a waste of compute .. and that was a mistake as i kept running into compiler errors. when i broke the code between first JPEG and the rest, i couldn't bridge them, the locality of variables became a problem. and then came the infamous "Segmentation faults". what is interesting is that when there is a segfault the compiler doesn't point you to the line or anything, it just saying Segmentation fault, core dumped. the reason interestingly is that segmentation faults happen when the OS runs the program and not when the compiler is compiling, very interesting. even when i made a single while loop for the first and the rest of JPEGs, i kept running into segfaults. what i learned is. FILE * is a pointer to a file, that can be assigned a name using the sprintf & fopen. but you have to use fwrite to actually write it. segfaults happen when you fwrite/fclose without opening a file. when the code skips directly to else condition or skips the while loop directly and goes to close, that's what creates segfaults. i rewrote the code to this problem 3 times, which is crazy but it felt important. if i had spare time today i thought of rewriting filter-more from scratch but i don't have time. maybe i'll review it at the end of the course. 

### Day 23: July 29, 2026
**Today's Progress**: tried solving recover problem of week 4.
**Thoughts**: It felt easy from the guided video and the pseudocode given. wrote just the beginning. 

### Day 22: July 28, 2026
**Today's Progress**: wrote test txt for tideman.
**Thoughts**: It is so much better to write a text file for a program like tideman. last month i tested the program manually, it took me hours. 

### Day 21: July 27, 2026
**Today's Progress**: rewrote tideman's lock_pairs using recursion.
**Thoughts**: I wanted to clear this backlog before rewriting entire filer-more problem. surprisingly it took me a whole hour just to read and recall what i wrote just a month ago. i wrote some blunders and only realised it now. i just couldn't write the recursion code, so i copied it from Gemini, only to realise how simple it was. it is basically a reverse for loop. its like a fractal that keeps on zooming as long as the base condition is true. very interesting. but it is way above any student's intuition i feel. 

### Day 20: July 26, 2026
**Today's Progress**: solved filter-more pset of lecture 3.
**Thoughts**: edge detection was technically difficult. my intuition was if a pixel is different in colour compared to a neighbouring left and right pixels then it should be given a lighter colour and darker if its not. only it should be done in all directions. the formula given by CS50 is hard to understand and executing it is not easy. i will rewrite the code, not just edge detection but the entire program, which i don't think is necessary but it will be fun as i am creating an entirely new file, calling memory and giving it back. maybe then i can go watch dave's garage video on malloc.

### Day 19: July 25, 2026
**Today's Progress**: solved volume and filter-less pset of lecture 4.
**Thoughts**: The volume problem was easy relatively speaking but working with data types you don't even know exists threw me off. i guess after a while of doing small projects i will have an understanding of different things generally used but for this one i had no idea i have to use int16_t and then convert the int factor to float. so, i had white noise or hum noise coming in the output file until i used the correct data type and float for the factor. and these were not discussed in the lecture, not that they should discuss everything before hand, it feels like shooting arrows in the dark as a beginner to do this by myself.
the filter-less problem was fun honestly. i was intrigued by the idea rather than the code. grey-scaling is just having equal amount of RGBs, it didn't occur to me and now i'm interested to know how exactly black and white pictures and movies are colourised. reflection is easy and fun. sepia is boring as the answers were given already, there was nothing to do. blur was simple but again the conception of the solution was more interesting and cs50 gives away the idea of making a copy first which i feel students should figure out. 

### Day 18: July 24, 2026
**Today's Progress**: watched lecture 4 of CS50x: memory.
**Thoughts**: It is illuminating to see how memory works, at least in the context of coding. some of the comments said it was a difficult lecture to follow but i had no problem. i wish the lecture was twice as long and gave more examples right in the lecture and i don't question whether something was taught when i am solving the problems. honestly it stirred my curiosity on how the cpu is traversing the memory in the first place, and have a basic understanding of cpu and memory. its all really exciting.

### Day 17: June 19, 2026
**Today's Progress**: solved tideman pset of lecture 3.
**Thoughts**: and that was the peak, not the entire problem but just the locked pairs function which is basically a search algorithm. I intuitively wrote a bfs algorithm even though the walkthrough video and ai told me to use recursion with dfs. this problem have both a sorting algorithm and a search algorithm in it, great way to make me eat programming vegetables. it took me close to 4,5 hours to come up with bfs for the locked pairs function, rest of the problem was relatively easy. i almost gave up because i had no clue how i would solve it. in retrospection i'm glad i didn't look up the answer, then i would've missed the fun. i had some idea how to do it and that is what helped me. tip to my future self. whatever clue you have filter it, think it through with examples, use pen and paper and then ask ai. no way you will not find an answer. except for a few syntax error the code compiler without any logical errors that was very satisfying. now off to learning how to solve it using recursion.

### Day 16: June 15, 2026
**Today's Progress**: solved runoff pset of lecture 3.
**Thoughts**:phew! this was by far the hardest despite half the code and most of the structure was given to me in the question. Every single function was hard and i had to pulg the output of each into another. debugging it was a nightmare. debug50 didn't start most of the time. when it did, i had to manually give test data so many times, it taught me patience. at the end it felt like a simple solution but with multiple parts. I solved it over multiple days, i think it took more than a day. let's get to the next pset - the final boss: Tideman!

### Day 15: May 25, 2026
**Today's Progress**: solved plurality pset of lecture 3.
**Thoughts**: very interesting. although it helped that the code was well written and commented i can imagine how hard it is to read badly written code and make changes. to find out the candidate with the highest votes i used bubble sortting but just once loop. the condition was to print winner or miltiple winners. it was interesting how to do that. i first figuredou the highest votes and then wrote one more for loop to go find if there are any one with matching votes, but there is a risk if reprinting the winner. to circumvent that i wrote an if condition that checks the name first and then proceed to the votes. nice problem.

### Day 14: May 24, 2026
**Today's Progress**: solved sort pset of lecture 3.
**Thoughts**: pretty easy one. run the program and check time it took and you can see the pattern of the speeds, the bigOs and omegas.

### Day 13: May 23, 2026
**Today's Progress**: actually finished lecture 3.
**Thoughts**: just that. i was introduced to recursion, very interestng. i visualise it as the same function being nest in itself every time it loop through until it reaches the base condition. when it does reach then it has to execute this massive amount of code. when i shared this with gemini, it called my intution sharp. and it was the reason recursion was used in few cases where the data itself is nested like that and for generally purposes regular while/for loop would be better and safe as recursion will lead to wait for it ... "stack overflow". it is a special day, i learned what recursion and stackoverflow means on the same day. i'm really enjoying this! and i actually learned what a "logarithm" is. now i will never forget what a logarithm is.

### Day 12: May 22, 2026
**Today's Progress**: watched lecture 3 of cs50x.
**Thoughts**: the lecture is named algorithms. it wasn't deep like the lectures so far, looking forward to the psets.

### Day 11: May 21, 2026
**Today's Progress**: Finished psets of week 2 - substitution.
**Thoughts**: I had to write a for loop inside a for loop. the code should check if a char in the key is alphabetic and also non-repeating. It was interesting and actually quite simple. That's it, other than that the substitution was simple. but it take me about 3 hours to do it.

### Day 10: May 20, 2026
**Today's Progress**: Finished psets of week 2 - caesar.
**Thoughts**: This pset took a lot of time. but more than time i felt exhausted after trying to wrap my head around it after 3 hours. i took a break and finished it with AI's help and using debug50. interesting thing is that dubugging tool did not help me as i didn't notice that argv is a string and you cannot use it directly to add to the plaintext. you have to first convert it to int using atoi. just getting comfortable with command line argument syntax took some time and then i had to write code navigating all cases of input in those arguments. since that is the first thing you have to do when a program gets executed, I had to think differently. then you have to nest your actual program in the argument navigation. it was tough to hold all the complexity for the first few hours but i eventually got to the solution. It feels very fulfilling to finally compile and get the test results right. I'm trying to rewrite my code and this time i got it compiled in the first try the second time i wrote it. i didn't even feel the need to write it once more. I read the substitution problem and it feels similar to caesar in the command line argument navigation but i need to think about how i can check for repeating letters in argument input. then i just have to use the argv array to encrypt. seems like a 2h pset. let's see. 

### Day 9: May 19, 2026
**Today's Progress**: Finished psets of week 2 - Scrabble, Readability.
**Thoughts**: Like credit i wrote a manual if else for each alphabet, the code was 275 lines meanwhile the efficient code of it was 50 lines, i was shocked to see it. wrote an if function that check if the char is an alphabet, turns out there is one such function isalpha() in ctype.h. I thought about how i could map the scores to alphabets but couldn't think of any idea. turns out you just have to make an array of the scores and access that array using the relative position of the alphabet and sum up the scores. even though this is meant to be an easy pset it was challenging for me. Coming to readability, this felt easy and i could finish it in an hour. i didn't think about the letters, words, sentences being integers and dividing them would truncate the value. so, you should use floats. not only that, i also forgot to round off the coleman liau index.

### Day 6 - 3: May 16 - 18, 2026
**Today's Progress**: Watched cs50x lecture 2, rewrote credit for practice along with lecture 2's examples
**Thoughts**: Not much progress for the 3 days. struggling with following a daily schedule, the result being not much time to code. Seems to me, I have to really protect my time from others & more importantly my own impulse to just procrastinate. Anyway, I rewrote credit for the 3rd time as a practice of logic & more importantly syntax. I heard from someone that the code their projects 3 times; first to make it happen, second to polish & third to let it sink to your subconscious mind. although it sound unnecessary, it takes very little time the 3rd time. 2nd time is where you get the most value but 3rd time feels like a nostalgic cruise through a neighboorhoob you've lived in. Hopefully the next week is more productive and week 3, 4 & 5 are really the hardest parts of the course from what i hear.

### Day 5: May 15, 2026
**Today's Progress**: Debugged credit pset's code.
**Thoughts**: Had only 1 hour to code today. so, I decided to just debug the code i wrote yesterday. learned about stopping the code using "return 0;". More interestingly there was a bug in the code, output was not as desired. but i was very sure my code was flawless. turns out i was right my code was not the problem, the problem was .. the input. I was copying the input numbers from else where and there some spaces at the end of those numbers that i didn't notice. funny!

### Day 4: May 14, 2026
**Today's Progress**: using loops in proper place, rewrote the entire code of credit pset.
**Thoughts**: didn't have much time today, spent couple of hours on rewriting the credit code. interestingly i took a whole hour to write a single loop that checks for a positive 13, 15 or 16 digit number. i was impressed how quickly i wrote the rest of the code that include main sum logic. to my surprise the code compiled in a single try, unbelievable. but there are bugs. it gives wrong output in some cases. i need to check it again.

### Day 3: May 13, 2026
**Today's Progress**: Finished second part of the mario problem & cash problem. Finished major portion of the credit problem.
**Thoughts**: mario part was cakewalk. it took less than a minute, all i had to do was repeat the meat in the loop but flip it around so that hashes get printed first followed by spaces. the cash problem was interesting; although the description used big words like greedy algorithm, it was easy . but the credit problem was .. i surprised when i learned that we have to use peeling & shortening. they are creative ways of using what tools you have at hand but i have a feeling that there are more tools that make it so much easier to solve the same problem. it was too much for some one who just learning the basics of basics of their first programming language. so, i wrote the worst code when i manually pick each digit and assinged a variable for each one of them and the summed up that takes 2 moniters to see one line of code. It took me 6 hours to write inefficient code, i felt amazing! learning to code so far i have notice a cycle where i'm given a problem, i have no idea how to solve it. i logically deduct the problem and fit in the pieces of syntax i learned, this requires concentration and you being a nerd. then there is the struggle of getting your ideas to work .. and fail .. and fail .. and try again .. and again until you are cornered. slowly it works, i always find the solution, so far. its real joy. then back to square one with a new problem. i think the more iterations you go through of this the more it become second nature and you develop what people generally refer to as skill or worse talent. solving this credit problem was hard but fulfilling.

### Day 2: May 12, 2026
**Today's Progress**: Finished the mario part of Pset 1 of CS50x.
**Thoughts**: I ran into a couple of problems. I knew i just have to calculate the number of spaces and hashes for each row, embed these in a printf statement that is nested in a for loop. my first problem was that every row was row 1 repeated. so, the code was not updating the spaces and hashes for each row. fot this gemini suggestd me to use nested loop for the hashes, which worked but i ran into second problem where the last row had an unintended space at the beginning. Gemini told me to use use "" instead of " ". even though i was multiplying " " with 0, c was still printing a space.

### Day 1: May 11, 2026
**Today's Progress**: Finished lecture 1 of CS50x.
**Thoughts**: It was a good refresher of c syntax.

### Day 0: May 10, 2026
**Today's Progress**: Finished lecture 0 of CS50x.
**Thoughts**: I had watched the first two lectures of cs50x before. The Pset was to make a program in scratch for which i had an idea for last time which was to make a clicking game where you are ozzy ozbourne who has to fend off bats.i felt lazy and skipped this pset for now.
**Link**:
