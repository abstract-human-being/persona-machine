# Persona-Machine
A machine impersonating a person.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: How would you interpret that, Giambattista-Vico?" \
  | uvx persona-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install persona-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
persona-machine -a multilogue.txt
```
Or:
```bash
persona-machine multilogue.txt > response.txt
```
Or:
```bash
persona-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import persona_machine
```
