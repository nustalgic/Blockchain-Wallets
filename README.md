# Module-19-Challenge

[![Screen-Shot-2022-05-15-at-11-34-38-PM.png](https://i.postimg.cc/QCvYNzXz/Screen-Shot-2022-05-15-at-11-34-38-PM.png)](https://postimg.cc/ZvFxVVvP)

# Background

In this challenge I work at a startup that is building a new and disruptive platform called Fintech Finder. Fintech Finder is an application that its customers can use to find fintech professionals from among a list of candidates, hire them, and pay them. As Fintech Finder’s lead developer, you have been tasked with integrating the Ethereum blockchain network into the application in order to enable your customers to instantly pay the fintech professionals whom they hire with cryptocurrency.

The code enables your customers to send cryptocurrency payments to fintech professionals. To develop the code and test it out, you will assume the perspective of a Fintech Finder customer who is using the application to find a fintech professional and pay them for their work.

---

## Technologies

We'll be using Python and the following libraries to run and read our data. 

* [Streamlit](https://streamlit.io/)  - turns data scripts into shareable web apps in minutes. All in pure Python. No front‑end experience required.

* [Data Classes](https://docs.python.org/3/library/dataclasses.html)  - provides a decorator and functions for automatically adding generated special methods.

* [web3](https://web3py.readthedocs.io/en/stable/) - Web3.py is a Python library for interacting with Ethereum.


## Installation Guide

In order for us to get the data we need we must import proper libraries.

```python
import streamlit as st
from dataclasses import dataclass
from typing import Any, List
from web3 import Web3
```

---
## Usage
* Create additional user input areas in the Streamlit application. 

```python
def get_people():
    """Display the database of Fintech Finders candidate information."""
    db_list = list(candidate_database.values())

    for number in range(len(people)):
        st.image(db_list[number][4], width=200)
        st.write("Name: ", db_list[number][0])
        st.write("Ethereum Account Address: ", db_list[number][1])
        st.write("FinTech Finder Rating: ", db_list[number][2])
        st.write("Hourly Rate per Ether: ", db_list[number][3], "eth")
        st.text(" \n")
```
---

[![Screen-Shot-2022-05-15-at-11-13-29-PM.png](https://i.postimg.cc/Jzp7T3KF/Screen-Shot-2022-05-15-at-11-13-29-PM.png)](https://postimg.cc/cv8NCnp7)

[![Screen-Shot-2022-05-15-at-11-13-53-PM.png](https://i.postimg.cc/Lsh9Gqb8/Screen-Shot-2022-05-15-at-11-13-53-PM.png)](https://postimg.cc/945H7f26)

[![Screen-Shot-2022-05-15-at-11-12-47-PM.png](https://i.postimg.cc/02qNrybV/Screen-Shot-2022-05-15-at-11-12-47-PM.png)](https://postimg.cc/QV0Dysg7)



---

## Contributors

Brought to you by Elgin Braggs Jr.

---
## License

MIT