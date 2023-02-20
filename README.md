# BERT for EdTech

### BERT is trained on a masked-language-modeling task, which is essentially a giant multiple choice question. Here we've created a fun little script for generating multiple choice questions. As a language teacher, I personally use this program to make bespoke exams for my students.

```
text = "The visit had not been announced, but did not come as a complete surprise. For at least a fortnight rumours have swirled around Kyiv that the leader of the free world might extend a planned trip to Poland to Ukraine, too."
answer = "swirled"
top_k = 5000 ## number of words to choose from
offset = 1000 ## distance from plausible answers
choices = 5 ## number of alternative answers

generate_multiple_choice_questions(text, answer, top_k=500, offset=100, choices=5)

[OUTPUT]

QUESTION: The visit had not been announced, but did not come as a complete surprise. For at least a fortnight rumours have  ___________  around Kyiv that the leader of the free world might extend a planned trip to Poland to Ukraine, too.

A. arose
B. awakened
C. hardened
D. roaming
E. swirled
F. stalked

CORRECT ANSWER: swirled

```

### This is a simple tool that can be incorporated into a variety of ed-tech pipelines.
