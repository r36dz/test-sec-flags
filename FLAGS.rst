Flags
=====

Defaults
--------
makepkg.conf already defines the following:

- CPPFLAGS= -D_FORTIFY_SOURCE=2
- CFLAGS= -fstack-protector-strong
- CXXFLAGS= -fstack-protector-strong
- LDFLAGS= -z,relro

All tests will include -D_FORTIFY_SOURCE=2

Proposed
--------
- (Current Arch Flags) -fstack-protector-strong and partial relro
- (Current Arch Flags) -fstack-protector-strong and partial relro + stack-check
- -fstack-protector-strong and partial relro + PIE
- -fstack-protector-strong and partial relro + PIE + stack-check
- -fstack-protector-strong and PIE + full RELRO
- -fstack-protector-strong and PIE + full RELRO + stack-check
- -fstack-protector-strong and PIE + full RELRO + no-plt
- -fstack-protector-strong and PIE + full RELRO + no-plt + stack-check
