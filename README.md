# Theine 
[![Gem Version](https://badge.fury.io/rb/theine2.svg)](https://badge.fury.io/rb/theine2)

Theine is a Rails application pre-loader designed to work on JRuby.
It is similar to Zeus, Spring and Spork. The problem with Zeus and Spring is
that they use `fork` which doesn't work on JRuby.
```
  time rails runner "puts Rails.env"
  48.31s user 1.96s system 242% cpu 20.748 total  # normal
  time theine runner "puts Rails.env"
  0.12s  user 0.02s system 32%  cpu 0.449  total  # Theine
```
Docs https://theine2.readthedocs.io/en/latest
