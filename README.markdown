~~~haskell

-- zero
0 ≔ ∀ t. t

-- one
1 ≔ ∀ t. t → t

-- two
2 ≔ ∀ t. t → t → t

-- +1
succ n ≔ ∀ t. t → n {t ≔ t}

-- three
3 ≔ succ 2

-- four
4 ≔ succ 3

-- multiplication
a ⋅ b ≔ ∀ t. (a → b → t) → t

-- division
a / b ≔ ∃ c. a = b ⋅ c

-- addition
a + b ≔ ∀ t. (a → t) → (b → t) → t

-- subtraction
a - b ≔ ∃ c. a = b + c

-- negation
-a ≔ 0 - a

-- exponentiation
a ^ b ≔ b → a

-- square
sqr a ≔ a ⋅ a

-- square root
sqrt a ≔ ∃ b. a = sqr b

-- logarithm
log b a ≔ ∃ c. a = b ^ c

-- complement
¬a ≔ 0 ^ a

-- and
a ∧ b ≔ a ⋅ b

-- xor
a ⊕ b ≔ a + b

-- or
a ∨ b ≔ (a ∧ b) ⊕ a ⊕ b

~~~
