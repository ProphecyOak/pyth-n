Lexer reads through code to create tokens.
`Grammar/Tokens` is read by `Tools/build/generate_token.py` to create `Include/internal/pycore_token.h` and `Parser/token.c`
`Parser/token.c` is used by `Parser/lexer/lexer.c` to check for special tokens using `Include/internal/pycore_token.h`
`Parser/lexer/lexer.c` takes the code and creates the tokens for the AST
