## 1.2-2
	$8n^2 = 64n \cdot \ln{n}$
	$0 = (64\ln{n} - 8n)n$
	$64\ln{n}-8n = 0$
	$8\ln{n}-n = 0$
	$8=\frac{n}{\ln{n}}$
	We want $8 > \frac{n}{\ln{n}}$
	n = 0-26

## 1.2-3
	$100n^2<2^n$
	$\ln{100} + 2\ln{n} < n\ln{2}$
	$4.6 + 2\ln{n}< n0.7$
	$6.57 + 2.85\ln{n} < n$
	$6.57 < n - 2.85\ln{n}$

## 2.1-2
	Initilization: Sum is = 0 for i = 1 to n. Since there is nothing to sum yet, the total is 0.
	Maintenance: If we take the prior sum, and add the current index A[i]. The sum is the total of A[1] + ... + A[i]
	Termination: Once the loop reach i = n. Loop terminates and we have total sum of the full array A[1:n] keeping invariance.
