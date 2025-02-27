We start with building the theory of divisibility in the integers.


# Definition 2.1:

1.  Suppose $ a, b \in \mathbb{Z} $ , we say that $ b $ divides $ a $ (written $ b \mid a $) when there exists $ c \in \mathbb{Z} $ such that $ a = bc $. Then, we also say that $ a $ is divisible by $ b $ or $ b $ is a divisor of $ a $.

2.  When $ a $ is not divisible by $ b $, then we write $ b \nmid a $.

3.  When $ b $ divides $ a $ and $ 1 \leq b < a $, we say $ b $ is a proper divisor of $ a $.

4.  We write $ a^k \mid \mid b $ when $ a^k \mid b $ but $ a^{k+1} \nmid b $.

We note $ b \mid a $ only makes sense when $ b \neq 0 $.


## Example

$ 4 \mid \mid 24 $ because $ 4 \mid 24 $ and $ 4^2 \nmid 24 $ ($ 8 \mid 24 $).


# Theorem 2.2:

1.  $ a \mid a $ for every $ a \in \mathbb{Z} \backslash \{0\} $.
2.  $ a \mid 0 $ for every $ a \in \mathbb{Z} \backslash \{0\} $.
3.  If $ a \mid b $ and $ b \mid c $, then $ a \mid c $.
4.  If $ a \mid b $ and $ b \mid a $, then $ a = \pm b $.
5.  If $ a \mid b $ and $ a \mid c $, then for all $ x, y \in \mathbb{Z} $, one has $ a \mid bx + cy $. (\*)
6.  If $ a \mid b $ and $ a > 0 $ and $ b > 0 $, then $ a \leq b $.
7.  When $ m \neq 0 $, one has $ a \mid b \iff ma \mid mb $.


# Theorem 2.3: (The Division Algorithm)

For any $ a, b \in \mathbb{Z} $ and $ a > 0 $, there exist <span class="underline">unique</span> $ q, r \in \mathbb{Z} $ with $ b = qa + r $ and $ 0 \leq r < a $. If further, one has $ a \not | \: b $, then one has $ 0 < r < a $.


## Proof


### Existence

We can prove existence of such $ q, r $ by construction.

We define $ q $ so that $ a q = \max_q \{a q \: | \: a q \leq b\} $, and let $ r = b - a q $.

Now, $ a(q + 1) > b \implies aq + a > b \implies a > b - a q = r $. So, we have found $ r $ such that $ 0 \leq r < a $.


### Uniqueness

To prove uniqueness, suppose there exist $ q, r, q', r' $ such that $ b = qa + r $ and $ b = q'a + r' $ with $ r \neq r' $. WLOG assume $ r < r' $.

Then, we have $ qa + r = q'a + r' \implies (q - q')a = r' - r $.

This means $ a \mid (r' - r) $. We also have $ 0 \leq r, r' < a \implies 0 \leq r' - r < a $.

But because divisors are smaller than the number they divide, we have $ r' - r < a $. This is a contradiction which means our assumption that $ r \neq r' $ is wrong. Hence, $ r = r' $.


# Definition 2.4:

1.  Suppose that $ a \in \mathbb{Z} \backslash \{0\} $ and $ b, c \in \mathbb{Z} $. Then we say $ a $ is a <span class="underline">common divisor</span> of $ b $ and $ c $ when $ a \mid b $ and $ a \mid c $.

2.  When $ b $ and $ c $ are not <span class="underline">both</span> 0, the number of common divisors of $ b $ and $ c $ is finite (**Theorem 2.2 (vi)**). So, we can define the <span class="underline">greatest common divisor</span> (or <span class="underline">highest common factor</span>) of $ b $ and $ c $ to be the largest common divisor. The $ \gcd $ of $ b $ and $ c $ is written $ (b, c) $ (or $ \gcd(b, c) $).

3.  When $ g_1, \ldots, g_n $ are integers, not all 0, write $ (g_1, \ldots, g_n) $ for the largest integer $ g $ with the property that $ g \mid g_i (1 \leq i \leq n) $.


## Example

$ (0, 2) = 2 $, $ (1, 3) = 1 $, $ (1729, 182) = 91 $
