Module | Notation | Definition | Level | Associativity
---|---|---|---|---
`FunNotation` | `begin e1 end` | `e1` | 0 |
`FunctorNotation` | `f <$> x` | `fmap f x` | 52 | left
`ApplicativeNotation` | `f <*> x` | `ap f x` | 52 | left
`MonadPlusNotation` | `x <+> y` | `mplus x y` | 54 | left
`MonadNotation` | `c >>= f` | `bind c f` | 58 | left
`MonadNotation` | `f =<< c` | `bind c f` | 61 | right
`MonadNotation` | `f >=> g` | `mcompose f g` | 61 | right
`MonadNotation` | `x <- c1 ;; c2` | `bind c1 (fun x => c2)` | 61 | right
`MonadNotation` | `' pat <- c1 ;; c2` | `bind c1 (fun x => match x with pat => c2)` | 61 | right
`MonadNotation` | `e1 ;; e2` | `_ <- e1 ;; e2` | 61 | right
`FunNotation` | `f $ x` | `f x` | 99 | right
