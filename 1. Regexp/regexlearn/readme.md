1. Intro									OK
2. What is Regular Expressions Regex?				^\w+\.pdf$
3. Basic Matchers								curious
4. Dot .: Any Character							.
5. Character Sets [abc]			 				b[aeiou]r
6. Negated Character Sets [^abc]					b[^eo]r
7. Letter Range[a-z]							[e-o]
8. Number Range[0-9]							[3-6]
9. Practice
10. Practice: Basic Matcher						of
11. Practice: Any Character						.
12. Practice: Character Sets						[bdf]eer
13. Practice: Negated Character Sets				be[^ou]r
14. Practice: Letter Range						[g-k]
15. Practice: Number Range						[2-7]
16. Practice completed!
17. Repetitions 
18. Repetitions: Asterisk						be*r
19. Plus Sign +								be+r
20. Question Mark ?							colou?r
21. Curly Braces - 1							be{2}r
22. Curly Braces - 2							be{3,}r
23. Curly Braces - 3							be{1,3}r
24. Practice
25. Practice: Asterisk *						de*p
26. Practice: Plus Sign +						de+p
27. Practice: Question Mark ?						an?
28. Practice: Curly Braces - 1					[0-9]{4}		\d{4}
29. Practice: Curly Braces - 2					[0-9]{2,}		\d{2,}
30. Practice: Curly Braces - 3					[0-9]{1,4}		\d{1,4}
31. Practice completed!
32. Parentheses ( ): Grouping						(haa)
33. Referencing a Group							(ha)-\1,(haa)-\2
34. Parentheses (?: ): Non-capturing Grouping			(?:ha)-ha,(haa)-\1
35. Pipe Character |							(C|c)at|rat
36. Escape Character \							(\*|\.)
37. Caret Sign ^: Selecting by Line Start				^[0-9]
38. Dollar Sign $: Selecting by End of Line			html$
39. Word Character \w: Letter, Number and Underscore		\w
40. Except Word Character \W						\W
41. Number Character \d							\d
42. Except Number Character \D					\D
43. Space Character \s							\s
44. Except Space Character \S						\S
45. Lookarounds								
46. Positive Lookahead: (?=)						\d+(?=PM)
47. Negative Lookahead: (?!)						\d+(?!PM)
48. Positive Lookbehind: (?<=)					(?<=\$)\d+
49. Negative Lookbehind: (?<!)					(?<!\$)\d+
50. Flags
51. Global Flag								/\w+\.com/g Mark the global check
52. Multiline Flag							/\w+\.com$/gm 			Mark the global and the multiline checks
53. Case-insensitive Flag						/\w+\.com$/gmi 			Mark the global, multine and the insensitive checks
54. Greedy Matching							.*r
55. Lazy Matching								.*?r
56. Congratulations, you have completed all the steps!				