# zhila
zhila, a polyglot static analysis tool.

## Usage

### Apply for Authorization
First, send an email to this mailbox `szhili365@outlook.com` to apply for authorization, and follow the steps in the replied email.

### Steps

1. Use `Dockerfile` or download [release pacakage](https://github.com/tuning003/zhila/releases/download/v1.1.5/zhila-linux_x86_64-v1.1.5.zip) directly;
2. Setup the License Server in a machine;
3. Use the CMD below.

### Command Line
```bash
# Test Case
INPUT_SERVICE=http://xxx INPUT_CHECK_CODE=xxx INPUT_LANGUAGE=cpp INPUT_FILES_PATH=test/files_path.txt INPUT_FAIL_ON_WARNINGS=true python3 ./src/main.py
```

### Github Action

1. Set github action secrets `SERVICE` and `CHECK_CODE`;
2. Create a `.github/workflow/zhila.yml` in the Github project. 
You can refer to the following two yml files, one is to analyze the incremental analysis of the list of diff files between versions, and the other is to analyze the full analysis of all code files.
    - [incremental analysis](https://github.com/szhili365/zhila/blob/main/.github/workflows/incremental.yml)
    - [full analysis](https://github.com/szhili365/zhila/blob/main/.github/workflows/full.yml)
