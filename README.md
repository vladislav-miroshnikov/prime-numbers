# Prime numbers checker
## Using Turing Machine
### Step 1
##### To generate free grammar (type T0) use command (inside "/TM_generator" folder):
```
python free_grammar_generator.py
```
By default, the following arguments are used:

TURING_MACHINE_PATH = "/TM_generator/TM.txt"

GRAMMAR_PATH = "/TM_generator/free_prime_grammar.txt"
##### To generate free grammar with specific arguments use:
```
free_grammar_generator.py [-h] [-tm TURING_MACHINE_PATH] [-g GRAMMAR_PATH]

optional arguments:
  -h, --help            Show this help message and exit
  -tm TURING_MACHINE_PATH, --turing_machine_path TURING_MACHINE_PATH
                        Path to turing machine file
  -g GRAMMAR_PATH, --grammar_path GRAMMAR_PATH
                        Output grammar path
```

### Step 2
##### To check if number is prime or not by grammar type T0 use command (inside "/TM_generator" folder):
```
python prime_checker.py -n N
```
N is a number to check

Sample:
```
python prime_checker.py -n 7
7 is a prime number
```
##### You can also specify your path to free grammar:
```
prime_checker.py [-h] [-g GRAMMAR_PATH] -n N

optional arguments:
  -h, --help            Show this help message and exit
  -g GRAMMAR_PATH, --grammar_path GRAMMAR_PATH
                        Path to file with grammar
```
By default, GRAMMAR_PATH = "/TM_generator/free_prime_grammar.txt"

File with results (applied productions) is prime_checker_result.txt file



