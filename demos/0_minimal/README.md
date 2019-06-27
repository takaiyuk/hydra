## Minimal example
The simplest possible example.

By default, the configuraiton object you will receive here is empty:
```text
$ python demos/0_minimal/minimal.py
[2019-06-24 18:33:02,542][__main__][INFO] - CWD: /private/home/omry/dev/hydra/outputs/2019-06-24_18-33-02
[2019-06-24 18:33:02,542][__main__][INFO] - Configuration:
{}
```

But you can pass in arbitrary configuration from the command line and it will be converted to a tree
structure for you:
```text
$ python demos/0_minimal/minimal.py abc=123 hello.a=456 hello.b=5671
[2019-06-21 17:55:46,231][__main__][INFO] - CWD: /private/home/omry/dev/hydra/outputs/2019-06-21_17-55-46
[2019-06-21 17:55:46,231][__main__][INFO] - Configuration:
abc: 123
hello:
  a: 456
  b: 5671
```