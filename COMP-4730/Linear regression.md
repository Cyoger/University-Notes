Joint Probability:
P(X,Y) 
probability of X and Y

Conditional Probability:
P(X|Y)
probability of X given Y

P(A|B) = P(AB)/P(B) when P(B) > 0

P(AB) = P(A|B)P(B) = P(B|A)P(A)

P(AB) = P(A)P(B)

two events A and B are conditionally independent given C if they are independent after conditioning on C. 
P(AB|C) = P(B|AC)P(A|C) = P(B|C)P(A|C)

Example 


![[Pasted image 20231130015350.png]]

for this the question gives us the joint probability of students passing both the final and midterm or in notation P(FM) = 0.45
and the probability of students passing the final which is P(F) = 0.60
to find the probability or percent of students who passed final and also the midterm i.e. 
P(F|M), we use the conditional probability formula which is, P(F|M) = P(FM)/P(F)
0.45/0.60 = 0.75

Marginalization (Sum rule)
$$p(x) = \Sigma_y p(x,y)$$

Law of total probability
$$p(x) = \Sigma_y p(x|y).p(y)$$

## Bayes rule 

$$P(A|B) = P(AB)/P(B) (conditional probability)$$
 $$P(A|B) = P(B|A)P(A)/P(B)  (product rule)$$
 
$$ P(A|B) = P(B|A)P(A)/\Sigma P(B|A)P(A)$$
$$P(A/B) = P(A)P(B|A)/P(B)$$
$$P(B) = \Sigma_j P(B|A_j)P(A_j)$$
$$P(A|B) = P(A)P(B|A)/P(B)$$
$$p(\theta|x) = p(x|\theta)p(\theta)/p(x)$$
$$Posterior = likelihood * prior/evidence$$ $$Posterior\ probabolity\ \alpha\ Likelihood\ x Prior\ Probability$$

