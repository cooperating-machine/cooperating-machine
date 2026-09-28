# Cooperating-Machine
A Machine that cooperates.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: How do we cooperate here, machine?" \
  | uvx cooperating-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install cooperating-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
cooperating-machine -a multilogue.txt
```
Or:
```bash
cooperating-machine multilogue.txt > response.txt
```
Or:
```bash
cooperating-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import cooperating_machine
```
