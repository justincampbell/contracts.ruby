## v0.9
- (delete this line and add your changes here)

## v0.8
- code refactored (very slight loss of performance, big increase in readability)
- fail when defining a contract on a module without `include Contracts::Modules`
- fixed several bugs in argument parsing, functions with complex params get contracts applied correctly now.
- added rubocop to ci.
- if a contract is set on a protected method, it should not become public.
- fixed pattern matching when the multiple definitions of functions have different arities.
- couple of new built-in contracts: Nat, Eq.
- changed `Invariant` to `invariant`: `invariant(:day) { 1 <= day && day <= 31 }`
- prettier error messages (`Contracts::Num` is now just `Num`, for example)
- support for yard-contracts
