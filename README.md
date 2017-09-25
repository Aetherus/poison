# Poison

This is a fork from [devinus/poison](https://github.com/devinus/poison) to add more literals to JSON.

## DateTime

Add datetime literal to JSON.

A datetime literal is an RFC3339 string quoted with angle brackets.
e.g. `<2017-09-25 08:49:03.007407Z>`.

```elixir
Poison.encode!(DateTime.utc_now)
#=> "<2017-09-25 08:49:03.007407Z>"

Poison.decode!("<2017-09-25 08:49:03.007407Z>")
#=> #DateTime<2017-09-25 08:49:03.007407Z>
```
