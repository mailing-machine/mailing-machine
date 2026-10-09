# Mailing-Machine
A machine that sends and receives mail.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Mail all this, machine." \
  | uvx mailing-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install mailing-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
mailing-machine -a multilogue.txt
```
Or:
```bash
mailing-machine multilogue.txt > response.txt
```
Or:
```bash
mailing-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import mailing_machine
```
