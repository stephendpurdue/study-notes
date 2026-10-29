Elixir code is run during compile time.
.ex - compiled code.
.exs - interpreted code.
_ can be used before an argument to mute it.
@ can be used at the module level to ensure a variable won't change.

```
@x 5
```
Atoms can be used for constant values.

```
def main do
      name = "Stephen";
      status = Enum.random([:gold, :silver, :bronze])

      if status === :gold do
        IO.puts("Welcome to the gym, #{name}.")
      else
        IO.puts("Sorry, you cannot enter.")

      end
    end
```

