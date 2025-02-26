# The Operators

~ = NOT (!)
| p | ~p |
| - | -|
| T | F |
| F | T |

v = OR (||)

| p | q | p v q |
| - | -| - |
| F | F | F |
| F | T | T |
| T | F | T |
| T | T | T |

∧ = AND (&&)
| p | q | p ∧ q |
| - | -| - |
| F | F | F |
| F | T | F |
| T | F | F |
| T | T | T |

p -> q = p implies q

| p | q | p -> q |
| - | -| - |
| F | F | T |
| F | T | T |
| T | F | F |
| T | T | T |

p <-> q = (p equals q)
| p | q | p <-> q |
| - | -| - |
| F | F | T |
| F | T | F |
| T | F | F |
| T | T | T |
