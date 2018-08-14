Daniel Bank [Aug 8th at 9:50 PM]
Something that is bothering me:  Isn’t classification in essence still simply regression?  Two thoughts:

1) For example, the test score / grades problem where we calculate a score for a given (test_score, grades) point.  If it is ≥ 0, we say pass; if it is < 0, we say fail.  But essentially we are trying to predict quantity, which was what I understood the definition of regression to be

2) Is it true to say all regression problems are about predicting a quantity (i.e. a scalar value)?  Could we have regression problems that are trying to predict a vector?  (Without getting too far ahead of myself, I feel like this would be a further case for all classification problems being part of the set of regression problems).

I am sure this is all stemming from my naive understanding, but would appreciate to hear an expert’s take on my thinking (edited)


2 replies
Luke Rucks [7 hours ago]
In a classification problem with only two categories, it could probably be solved with a regression and then specifying a threshold above and below which classification is made, but this will only work for linear classifications (i.e. where the classification is a single smooth cut.)  This would fail in two broad categories:
1.  the cut isn't linear.  Very frequently, the boundary isn't linear.
2.  There are more than two categories.  Categories are not on a scale where those > a certain threshold are classified as a certain thing; there isn't a number above which something goes from a cat to a dog to a fox. (edited)


Luke Rucks [7 hours ago]
Regressions are also *usually* vectors, not scalars!
