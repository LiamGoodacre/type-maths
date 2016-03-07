~~~haskell

0 ≔ ∀ t. t

1 ≔ ∀ t. t → t

2 ≔ ∀ t. t → t → t

succ n ≔ ∀ t. t → n {t = t}

3 ≔ succ 2

4 ≔ succ 3

a ⋅ b ≔ ∀ t. (a → b → t) → t

a / b ≔ ∃ c. a = b ⋅ c

a + b ≔ ∀ t. (a → t) → (b → t) → t

a - b ≔ ∃ c. a = b + c

negate a ≔ 0 - a

a ^ b ≔ b → a

sqr a ≔ a ⋅ a

sqrt a ≔ ∃ b. a = b ⋅ b

log b a ≔ ∃ c. a = b ^ c

not a ≔ 0 ^ a

a & b ≔ a ⋅ b

xor a b ≔ a + b

a | b ≔ (a ⋅ b) + a + b

~~~
