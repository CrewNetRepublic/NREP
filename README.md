# About NREP
This is an exemplary, non-reference implementation of NREP/RecRoll.

NREP, NetREP is a decentralized data transmission network project designed for anonymous and secure interaction with the Internet and blocking bypass.
The main provisions of the NREP/RecRoll protocol are given in the [NREP_v0.1_reference](https://github.com/N1nthyesiam/NREP/blob/main/NREP_v0.1_reference.txt).

# Installation
You can use pip to install this package:
```pip install NREP```

You also can use the [wheel](https://github.com/N1nthyesiam/NREP/blob/Stable/dist/NREP-0.1.0-py3-none-any.whl) to install the package or install it via [PyPI](https://pypi.org/project/NREP/).

# Bit of theory
NREP redirects your traffic through several network nodes in such a way as to erase the maximum number of indirect signs.
For each connection (socket), a _pipe_ is created that passes through several nodes.

Different sets of nodes can be used for different connections, which increases anonymity and security (even when connected to the same server). 
The traffic required to create a pipe (handshake) is also encrypted in a special way.

Creating a pipe takes some time and piping is used to speed up the connection (one connection can be used for several consecutive requests).
On average, the difference in speed between direct connection and NREP pipe is ±5%
